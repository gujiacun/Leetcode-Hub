# $1242. [中等] 多线程网页爬虫

**题目链接：**[https://leetcode-cn.com/problems/web-crawler-multithreaded](https://leetcode-cn.com/problems/web-crawler-multithreaded)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给你一个初始地址&nbsp;<code>startUrl</code>&nbsp;和一个 HTML 解析器接口&nbsp;<code>HtmlParser</code>，请你实现一个&nbsp;<strong>多线程的网页爬虫</strong>，用于获取与&nbsp;<code>startUrl</code>&nbsp;有&nbsp;<strong>相同主机名&nbsp;</strong>的所有链接。&nbsp;</p> 
  <p>以&nbsp;<strong>任意&nbsp;</strong>顺序返回爬虫获取的路径。</p> 
  <p>爬虫应该遵循：</p> 
  <ul> 
   <li>从&nbsp;<code>startUrl</code>&nbsp;开始</li> 
   <li>调用&nbsp;<code>HtmlParser.getUrls(url)</code> 从指定网页路径获得的所有路径。</li> 
   <li>不要抓取相同的链接两次。</li> 
   <li>仅浏览与&nbsp;<code>startUrl</code>&nbsp;<strong>相同主机名&nbsp;</strong>的链接。</li> 
  </ul> 
  <p><img src="https://user-gold-cdn.xitu.io/2019/11/7/16e463265c7086cb?w=975&amp;h=266&amp;f=png&amp;s=24624" alt=""><img style="height:164px; width:600px" src="/aliyun-lc-upload/uploads/2019/11/09/urlhostname.png" alt=""></p> 
  <p>如上图所示，主机名是&nbsp;<code>example.org</code>&nbsp;。简单起见，你可以假设所有链接都采用&nbsp;<strong>http 协议</strong>，并且没有指定&nbsp;<strong>端口号</strong>。举个例子，链接&nbsp;<code>http://leetcode.com/problems</code> 和链接&nbsp;<code>http://leetcode.com/contest</code> 属于同一个&nbsp;<strong>主机名</strong>， 而&nbsp;<code>http://example.org/test</code>&nbsp;与&nbsp;<code>http://example.com/abc</code> 并不属于同一个&nbsp;<strong>主机名</strong>。</p> 
  <p><code>HtmlParser</code> 的接口定义如下：</p> 
  <pre class="language-text">interface HtmlParser {
  // Return a list of all urls from a webpage of given <em>url</em>.
  // This is a blocking call, that means it will do HTTP request and return when this request is finished.
  public List&lt;String&gt; getUrls(String url);
}</pre> 
  <p>注意一点，<code>getUrls(String url)</code>&nbsp;模拟执行一个HTTP的请求。 你可以将它当做一个阻塞式的方法，直到请求结束。&nbsp;<code>getUrls(String url)</code>&nbsp;保证会在&nbsp;<strong>15ms&nbsp;</strong>内返回所有的路径。 单线程的方案会超过时间限制，你能用多线程方案做的更好吗？</p> 
  <p>对于问题所需的功能，下面提供了两个例子。为了方便自定义测试，你可以声明三个变量&nbsp;<code>urls</code>，<code>edges</code>&nbsp;和&nbsp;<code>startUrl</code>。但要注意你只能在代码中访问&nbsp;<code>startUrl</code>，并不能直接访问&nbsp;<code>urls</code>&nbsp;和&nbsp;<code>edges</code>。</p> 
  <p>&nbsp;</p> 
  <p><strong>拓展问题：</strong></p> 
  <ol> 
   <li>假设我们要要抓取 10000 个节点和 10 亿个路径。并且在每个节点部署相同的的软件。软件可以发现所有的节点。我们必须尽可能减少机器之间的通讯，并确保每个节点负载均衡。你将如何设计这个网页爬虫？</li> 
   <li>如果有一个节点发生故障不工作该怎么办？</li> 
   <li>如何确认爬虫任务已经完成？</li> 
  </ol> 
  <p>&nbsp;</p> 
  <p><strong>示例 1：</strong></p> 
  <p><img style="height:287px; width:600px" src="/aliyun-lc-upload/uploads/2019/11/09/sample_2_1497.png" alt=""><img src="https://user-gold-cdn.xitu.io/2019/11/7/16e46559da0c446a?w=875&amp;h=418&amp;f=png&amp;s=43518" alt=""></p> 
  <pre class="language-text"><strong>输入：
</strong>urls = [
&nbsp; "http://news.yahoo.com",
&nbsp; "http://news.yahoo.com/news",
&nbsp; "http://news.yahoo.com/news/topics/",
&nbsp; "http://news.google.com",
&nbsp; "http://news.yahoo.com/us"
]
edges = [[2,0],[2,1],[3,2],[3,1],[0,4]]
startUrl = "http://news.yahoo.com/news/topics/"
<strong>输出：</strong>[
&nbsp; "http://news.yahoo.com",
&nbsp; "http://news.yahoo.com/news",
&nbsp; "http://news.yahoo.com/news/topics/",
&nbsp; "http://news.yahoo.com/us"
]
</pre> 
  <p><strong>示例 2：</strong></p> 
  <p><strong><img src="https://user-gold-cdn.xitu.io/2019/11/7/16e4657b399a5fd2?w=654&amp;h=431&amp;f=png&amp;s=33838" alt=""><img style="height:395px; width:530px" src="/aliyun-lc-upload/uploads/2019/11/09/sample_3_1497.png" alt=""></strong></p> 
  <pre class="language-text"><strong>输入：</strong>
urls = [
&nbsp; "http://news.yahoo.com",
&nbsp; "http://news.yahoo.com/news",
&nbsp; "http://news.yahoo.com/news/topics/",
&nbsp; "http://news.google.com"
]
edges = [[0,2],[2,1],[3,2],[3,1],[3,0]]
startUrl = "http://news.google.com"
<strong>输出：</strong>["http://news.google.com"]
<strong>解释：</strong>startUrl 链接与其他页面不共享一个主机名。</pre> 
  <p>&nbsp;</p> 
  <p><strong>提示：</strong></p> 
  <ul> 
   <li><code>1 &lt;= urls.length &lt;= 1000</code></li> 
   <li><code>1 &lt;= urls[i].length &lt;= 300</code></li> 
   <li><code>startUrl</code>&nbsp;是&nbsp;<code>urls</code>&nbsp;中的一个。</li> 
   <li>主机名的长度必须为 1 到 63 个字符（包括点 <code>.</code> 在内），只能包含从 “a” 到 “z” 的 ASCII 字母和 “0” 到 “9” 的数字，以及中划线 “-”。</li> 
   <li>主机名开头和结尾不能是中划线 “-”。</li> 
   <li>参考资料：<a href="https://en.wikipedia.org/wiki/Hostname#Restrictions_on_valid_hostnames">https://en.wikipedia.org/wiki/Hostname#Restrictions_on_valid_hostnames</a></li> 
   <li>你可以假设路径都是不重复的。</li> 
  </ul> 
 </div>
</div>

---

```java
/**
 * // This is the HtmlParser's API interface.
 * // You should not implement it, or speculate about its implementation
 * interface HtmlParser {
 *     public List<String> getUrls(String url) {}
 * }
 */
class Solution {
    public List<String> crawl(String startUrl, HtmlParser htmlParser) {
        
    }
}
```