# 1170. 比较字符串最小字母出现频次

**题目链接：**[https://leetcode-cn.com/problems/compare-strings-by-frequency-of-the-smallest-character](https://leetcode-cn.com/problems/compare-strings-by-frequency-of-the-smallest-character)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>我们来定义一个函数&nbsp;<code>f(s)</code>，其中传入参数&nbsp;<code>s</code>&nbsp;是一个非空字符串；该函数的功能是统计&nbsp;<code>s</code> &nbsp;中（按字典序比较）最小字母的出现频次。</p> 
  <p>例如，若&nbsp;<code>s = "dcce"</code>，那么&nbsp;<code>f(s) = 2</code>，因为最小的字母是&nbsp;<code>"c"</code>，它出现了&nbsp;2 次。</p> 
  <p>现在，给你两个字符串数组待查表&nbsp;<code>queries</code>&nbsp;和词汇表&nbsp;<code>words</code>，请你返回一个整数数组&nbsp;<code>answer</code>&nbsp;作为答案，其中每个&nbsp;<code>answer[i]</code>&nbsp;是满足&nbsp;<code>f(queries[i])</code>&nbsp;&lt; <code>f(W)</code>&nbsp;的词的数目，<code>W</code>&nbsp;是词汇表&nbsp;<code>words</code>&nbsp;中的词。</p> 
  <p>&nbsp;</p> 
  <p><strong>示例 1：</strong></p> 
  <pre class="language-text"><strong>输入：</strong>queries = ["cbd"], words = ["zaaaz"]
<strong>输出：</strong>[1]
<strong>解释：</strong>查询 f("cbd") = 1，而 f("zaaaz") = 3 所以 f("cbd") &lt; f("zaaaz")。
</pre> 
  <p><strong>示例 2：</strong></p> 
  <pre class="language-text"><strong>输入：</strong>queries = ["bbb","cc"], words = ["a","aa","aaa","aaaa"]
<strong>输出：</strong>[1,2]
<strong>解释：</strong>第一个查询 f("bbb") &lt; f("aaaa")，第二个查询 f("aaa") 和 f("aaaa") 都 &gt; f("cc")。
</pre> 
  <p>&nbsp;</p> 
  <p><strong>提示：</strong></p> 
  <ul> 
   <li><code>1 &lt;= queries.length &lt;= 2000</code></li> 
   <li><code>1 &lt;= words.length &lt;= 2000</code></li> 
   <li><code>1 &lt;= queries[i].length, words[i].length &lt;= 10</code></li> 
   <li><code>queries[i][j]</code>, <code>words[i][j]</code>&nbsp;都是小写英文字母</li> 
  </ul> 
 </div>
</div>

---

```java
class Solution {
    public int[] numSmallerByFrequency(String[] queries, String[] words) {
        
    }
}
```