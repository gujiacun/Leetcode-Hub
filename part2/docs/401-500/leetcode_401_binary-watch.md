# 401. [简单] 二进制手表

**题目链接：**[https://leetcode-cn.com/problems/binary-watch](https://leetcode-cn.com/problems/binary-watch)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>二进制手表顶部有 4 个 LED 代表<strong>小时（0-11）</strong>，底部的 6 个 LED 代表<strong>分钟（0-59）</strong>。</p> 
  <p>每个 LED 代表一个 0 或 1，最低位在右侧。</p> 
  <p><img style="height:300px" src="/wikipedia/commons/8/8b/Binary_clock_samui_moon.jpg"></p> 
  <p>例如，上面的二进制手表读取 “3:25”。</p> 
  <p>给定一个非负整数 <em>n&nbsp;</em>代表当前 LED 亮着的数量，返回所有可能的时间。</p> 
  <p><strong>案例:</strong></p> 
  <pre class="language-text">输入: n = 1
返回: ["1:00", "2:00", "4:00", "8:00", "0:01", "0:02", "0:04", "0:08", "0:16", "0:32"]</pre> 
  <p>&nbsp;</p> 
  <p><strong>注意事项:</strong></p> 
  <ul> 
   <li>输出的顺序没有要求。</li> 
   <li>小时不会以零开头，比如 “01:00”&nbsp;是不允许的，应为 “1:00”。</li> 
   <li>分钟必须由两位数组成，可能会以零开头，比如 “10:2”&nbsp;是无效的，应为 “10:02”。</li> 
  </ul> 
 </div>
</div>

---

```java
class Solution {
    public List<String> readBinaryWatch(int num) {
        
    }
}
```