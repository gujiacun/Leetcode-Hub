# 28. [简单] 实现 strStr()

**题目链接：**[https://leetcode-cn.com/problems/implement-strstr](https://leetcode-cn.com/problems/implement-strstr)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>实现&nbsp;<a href="https://baike.baidu.com/item/strstr/811469">strStr()</a>&nbsp;函数。</p> 
  <p>给定一个&nbsp;haystack 字符串和一个 needle 字符串，在 haystack 字符串中找出 needle 字符串出现的第一个位置 (从0开始)。如果不存在，则返回&nbsp; <strong>-1</strong>。</p> 
  <p><strong>示例 1:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> haystack = "hello", needle = "ll"
<strong>输出:</strong> 2
</pre> 
  <p><strong>示例 2:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> haystack = "aaaaa", needle = "bba"
<strong>输出:</strong> -1
</pre> 
  <p><strong>说明:</strong></p> 
  <p>当&nbsp;<code>needle</code>&nbsp;是空字符串时，我们应当返回什么值呢？这是一个在面试中很好的问题。</p> 
  <p>对于本题而言，当&nbsp;<code>needle</code>&nbsp;是空字符串时我们应当返回 0 。这与C语言的&nbsp;<a href="https://baike.baidu.com/item/strstr/811469">strstr()</a>&nbsp;以及 Java的&nbsp;<a href="https://docs.oracle.com/javase/7/docs/api/java/lang/String.html#indexOf(java.lang.String)">indexOf()</a>&nbsp;定义相符。</p> 
 </div>
</div>

---

```java
class Solution {
    public int strStr(String haystack, String needle) {
        
    }
}
```

```java
public class Solution {
    public int strStr(String haystack, String needle) {
        return haystack.indexOf(needle);
    }

//    public static void main(String[] args) {
//        String haystack1 = "hello", needle1 = "ll";
//        String haystack2 = "aaaaa", needle2 = "bba";
//        Solution28 solution = new Solution28();
//        System.out.println(solution.strStr(haystack1, needle1)); // 2
//        System.out.println(solution.strStr(haystack2, needle2)); // -1
//    }
}
```