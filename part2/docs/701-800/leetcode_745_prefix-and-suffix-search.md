# 745. [困难] 前缀和后缀搜索

**题目链接：**[https://leetcode-cn.com/problems/prefix-and-suffix-search](https://leetcode-cn.com/problems/prefix-and-suffix-search)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给定多个&nbsp;<code>words</code>，<code>words[i]</code>&nbsp;的权重为&nbsp;<code>i</code>&nbsp;。</p> 
  <p>设计一个类&nbsp;<code>WordFilter</code>&nbsp;实现函数<code>WordFilter.f(String prefix, String suffix)</code>。这个函数将返回具有前缀&nbsp;<code>prefix</code>&nbsp;和后缀<code>suffix</code>&nbsp;的词的最大权重。如果没有这样的词，返回 -1。</p> 
  <p><strong>例子:</strong></p> 
  <pre class="language-text"><strong>输入:</strong>
WordFilter(["apple"])
WordFilter.f("a", "e") // 返回 0
WordFilter.f("b", "") // 返回 -1
</pre> 
  <p><strong>注意:</strong></p> 
  <ol> 
   <li><code>words</code>的长度在<code>[1, 15000]</code>之间。</li> 
   <li>对于每个测试用例，最多会有<code>words.length</code>次对<code>WordFilter.f</code>的调用。</li> 
   <li><code>words[i]</code>的长度在<code>[1, 10]</code>之间。</li> 
   <li><code>prefix, suffix</code>的长度在<code>[0, 10]</code>之前。</li> 
   <li><code>words[i]</code>和<code>prefix, suffix</code>只包含小写字母。</li> 
  </ol> 
 </div>
</div>

---

```java
class WordFilter {

    public WordFilter(String[] words) {
        
    }
    
    public int f(String prefix, String suffix) {
        
    }
}

/**
 * Your WordFilter object will be instantiated and called as such:
 * WordFilter obj = new WordFilter(words);
 * int param_1 = obj.f(prefix,suffix);
 */
```