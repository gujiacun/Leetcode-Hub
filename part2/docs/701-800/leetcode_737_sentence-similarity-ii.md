# $737. [中等] 句子相似性 II

**题目链接：**[https://leetcode-cn.com/problems/sentence-similarity-ii](https://leetcode-cn.com/problems/sentence-similarity-ii)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给定两个句子 <code>words1, words2</code> （每个用字符串数组表示），和一个相似单词对的列表&nbsp;<code>pairs</code>&nbsp;，判断是否两个句子是相似的。</p> 
  <p>例如，当相似单词对是 <code>pairs = [["great", "fine"], ["acting","drama"], ["skills","talent"]]</code>的时候，<code>words1 = ["great", "acting", "skills"]</code> 和&nbsp;<code>words2 = ["fine", "drama", "talent"]</code> 是相似的。</p> 
  <p>注意相似关系是 <strong>具有</strong> 传递性的。例如，如果 "great" 和&nbsp;"fine" 是相似的，"fine" 和&nbsp;"good" 是相似的，则 "great" 和 "good" <strong>是相似的</strong>。</p> 
  <p>而且，相似关系是具有对称性的。例如，"great" 和 "fine" 是相似的相当于&nbsp;"fine" 和&nbsp;"great" 是相似的。</p> 
  <p>并且，一个单词总是与其自身相似。例如，句子 <code>words1 = ["great"], words2 = ["great"], pairs = []</code> 是相似的，尽管没有输入特定的相似单词对。</p> 
  <p>最后，句子只会在具有相同单词个数的前提下才会相似。所以一个句子 <code>words1 = ["great"]</code> 永远不可能和句子 <code>words2 = ["doubleplus","good"]</code> 相似。</p> 
  <p><strong>注：</strong></p> 
  <ul> 
   <li><code>words1</code> and <code>words2</code> 的长度不会超过&nbsp;<code>1000</code>。</li> 
   <li><code>pairs</code>&nbsp;的长度不会超过&nbsp;<code>2000</code>。</li> 
   <li>每个<code>pairs[i]</code>&nbsp;的长度为&nbsp;<code>2</code>。</li> 
   <li>每个&nbsp;<code>words[i]</code>&nbsp;和&nbsp;<code>pairs[i][j]</code>&nbsp;的长度范围为&nbsp;<code>[1, 20]</code>。</li> 
  </ul> 
 </div>
</div>

---

```java
class Solution {
    public boolean areSentencesSimilarTwo(String[] words1, String[] words2, List<List<String>> pairs) {
        
    }
}
```