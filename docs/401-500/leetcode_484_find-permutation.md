# $484. 寻找排列

**题目链接：**[https://leetcode-cn.com/problems/find-permutation](https://leetcode-cn.com/problems/find-permutation)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>现在给定一个只由字符 'D' 和 'I' 组成的 <strong>秘密签名</strong>。'D' 表示两个数字间的递减关系，'I' 表示两个数字间的递增关系。并且 <strong>秘密签名 </strong>是由一个特定的整数数组生成的，该数组唯一地包含 1 到 n 中所有不同的数字（秘密签名的长度加 1 等于 n）。例如，秘密签名 "DI" 可以由数组 [2,1,3] 或 [3,1,2] 生成，但是不能由数组 [3,2,4] 或&nbsp;[2,1,3,4] 生成，因为它们都不是合法的能代表&nbsp;"DI" <strong>秘密签名</strong> 的特定串。</p> 
  <p>现在你的任务是找到具有最小字典序的 [1, 2, ... n] 的排列，使其能代表输入的 <strong>秘密签名</strong>。</p> 
  <p><strong>示例 1：</strong></p> 
  <pre class="language-text"><strong>输入：</strong> "I"
<strong>输出：</strong> [1,2]
<strong>解释：</strong> [1,2] 是唯一合法的可以生成秘密签名 "I" 的特定串，数字 1 和 2 构成递增关系。
</pre> 
  <p>&nbsp;</p> 
  <p><strong>示例 2：</strong></p> 
  <pre class="language-text"><strong>输入：</strong> "DI"
<strong>输出：</strong> [2,1,3]
<strong>解释：</strong> [2,1,3] 和 [3,1,2] 可以生成秘密签名 "DI"，
但是由于我们要找字典序最小的排列，因此你需要输出 [2,1,3]。
</pre> 
  <p>&nbsp;</p> 
  <p><strong>注：</strong></p> 
  <ul> 
   <li>输出字符串只会包含字符 'D' 和 'I'。</li> 
   <li>输入字符串的长度是一个正整数且不会超过 10,000。</li> 
  </ul> 
  <p>&nbsp;</p> 
 </div>
</div>

---

**AC 代码：**

```java

```