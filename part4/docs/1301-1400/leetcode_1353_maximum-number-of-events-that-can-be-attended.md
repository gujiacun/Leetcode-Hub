# 1353. [中等] 最多可以参加的会议数目

**题目链接：**[https://leetcode-cn.com/problems/maximum-number-of-events-that-can-be-attended](https://leetcode-cn.com/problems/maximum-number-of-events-that-can-be-attended)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给你一个数组&nbsp;<code>events</code>，其中&nbsp;<code>events[i] = [startDay<sub>i</sub>, endDay<sub>i</sub>]</code>&nbsp;，表示会议&nbsp;<code>i</code>&nbsp;开始于&nbsp;<code>startDay<sub>i</sub></code>&nbsp;，结束于&nbsp;<code>endDay<sub>i</sub></code>&nbsp;。</p> 
  <p>你可以在满足&nbsp;<code>startDay<sub>i</sub>&nbsp;&lt;= d &lt;= endDay<sub>i</sub></code><sub>&nbsp;</sub>中的任意一天&nbsp;<code>d</code>&nbsp;参加会议&nbsp;<code>i</code>&nbsp;。注意，一天只能参加一个会议。</p> 
  <p>请你返回你可以参加的&nbsp;<strong>最大&nbsp;</strong>会议数目。</p> 
  <p>&nbsp;</p> 
  <p><strong>示例 1：</strong></p> 
  <p><img style="height: 400px; width: 600px;" src="/aliyun-lc-upload/uploads/2020/02/16/e1.png" alt=""></p> 
  <pre class="language-text"><strong>输入：</strong>events = [[1,2],[2,3],[3,4]]
<strong>输出：</strong>3
<strong>解释：</strong>你可以参加所有的三个会议。
安排会议的一种方案如上图。
第 1 天参加第一个会议。
第 2 天参加第二个会议。
第 3 天参加第三个会议。
</pre> 
  <p><strong>示例 2：</strong></p> 
  <pre class="language-text"><strong>输入：</strong>events= [[1,2],[2,3],[3,4],[1,2]]
<strong>输出：</strong>4
</pre> 
  <p><strong>示例 3：</strong></p> 
  <pre class="language-text"><strong>输入：</strong>events = [[1,4],[4,4],[2,2],[3,4],[1,1]]
<strong>输出：</strong>4
</pre> 
  <p><strong>示例 4：</strong></p> 
  <pre class="language-text"><strong>输入：</strong>events = [[1,100000]]
<strong>输出：</strong>1
</pre> 
  <p><strong>示例 5：</strong></p> 
  <pre class="language-text"><strong>输入：</strong>events = [[1,1],[1,2],[1,3],[1,4],[1,5],[1,6],[1,7]]
<strong>输出：</strong>7
</pre> 
  <p>&nbsp;</p> 
  <p><strong>提示：</strong></p> 
  <ul> 
   <li><code>1 &lt;= events.length &lt;= 10^5</code></li> 
   <li><code>events[i].length == 2</code></li> 
   <li><code>1 &lt;= events[i][0] &lt;= events[i][1] &lt;= 10^5</code></li> 
  </ul> 
 </div>
</div>

---

```

```