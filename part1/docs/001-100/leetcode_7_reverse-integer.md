# 7. [简单] 整数反转

**题目链接：**[https://leetcode-cn.com/problems/reverse-integer](https://leetcode-cn.com/problems/reverse-integer)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给出一个 32 位的有符号整数，你需要将这个整数中每位上的数字进行反转。</p> 
  <p><strong>示例&nbsp;1:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> 123
<strong>输出:</strong> 321
</pre> 
  <p><strong>&nbsp;示例 2:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> -123
<strong>输出:</strong> -321
</pre> 
  <p><strong>示例 3:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> 120
<strong>输出:</strong> 21
</pre> 
  <p><strong>注意:</strong></p> 
  <p>假设我们的环境只能存储得下 32 位的有符号整数，则其数值范围为&nbsp;[−2<sup>31</sup>,&nbsp; 2<sup>31&nbsp;</sup>− 1]。请根据这个假设，如果反转后整数溢出那么就返回 0。</p> 
 </div>
</div>

---

```java
class Solution {
    public int reverse(int x) {

    }
}
```

```java
class Solution {
    public int reverse(int x) {
        String str = String.valueOf(x);
        boolean isSub = str.charAt(0) == '-';
        long res;
        if (!isSub) {
            res = Long.parseLong(new StringBuilder(str).reverse().toString());
        } else {
            res = -Long.parseLong(new StringBuilder(str.substring(1)).reverse().toString());
        }
        if (res >= Integer.MIN_VALUE && res <= Integer.MAX_VALUE) {
            return (int) res;
        } else {
            return 0;
        }
    }

//    public static void main(String[] args) {
//        Solution7 solution = new Solution7();
//
//        System.out.println(solution.reverse(123)); // 321
//        System.out.println(solution.reverse(-123)); // -321
//        System.out.println(solution.reverse(120)); // 21
//        System.out.println(solution.reverse(1534236469)); // 0
//    }
}
```
