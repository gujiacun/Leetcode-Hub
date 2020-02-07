# 712. 两个字符串的最小ASCII删除和

**题目链接：**[https://leetcode-cn.com/problems/minimum-ascii-delete-sum-for-two-strings](https://leetcode-cn.com/problems/minimum-ascii-delete-sum-for-two-strings)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给定两个字符串<code>s1, s2</code>，找到使两个字符串相等所需删除字符的ASCII值的最小和。</p> 
  <p><strong>示例 1:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> s1 = "sea", s2 = "eat"
<strong>输出:</strong> 231
<strong>解释:</strong> 在 "sea" 中删除 "s" 并将 "s" 的值(115)加入总和。
在 "eat" 中删除 "t" 并将 116 加入总和。
结束时，两个字符串相等，115 + 116 = 231 就是符合条件的最小和。
</pre> 
  <p><strong>示例&nbsp;2:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> s1 = "delete", s2 = "leet"
<strong>输出:</strong> 403
<strong>解释:</strong> 在 "delete" 中删除 "dee" 字符串变成 "let"，
将 100[d]+101[e]+101[e] 加入总和。在 "leet" 中删除 "e" 将 101[e] 加入总和。
结束时，两个字符串都等于 "let"，结果即为 100+101+101+101 = 403 。
如果改为将两个字符串转换为 "lee" 或 "eet"，我们会得到 433 或 417 的结果，比答案更大。
</pre> 
  <p><strong>注意:</strong></p> 
  <ul> 
   <li><code>0 &lt; s1.length, s2.length &lt;= 1000</code>。</li> 
   <li>所有字符串中的字符ASCII值在<code>[97, 122]</code>之间。</li> 
  </ul> 
 </div>
</div>

---

**AC 代码：**

```java

```