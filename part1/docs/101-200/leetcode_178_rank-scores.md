# 178. 分数排名

**题目链接：**[https://leetcode-cn.com/problems/rank-scores](https://leetcode-cn.com/problems/rank-scores)

---

<div class="content__1Y2H">
 <div class="sql-schema-wrapper__1jqS">
  <a class="sql-schema-link__1VAC">SQL架构
   <svg viewbox="0 0 24 24" width="1em" height="1em" class="css-1lc17o4-icon">
    <path fill-rule="evenodd" d="M10 6L8.59 7.41 13.17 12l-4.58 4.59L10 18l6-6z"></path>
   </svg></a>
 </div>
 <div class="notranslate">
  <p>编写一个 SQL 查询来实现分数排名。如果两个分数相同，则两个分数排名（Rank）相同。请注意，平分后的下一个名次应该是下一个连续的整数值。换句话说，名次之间不应该有“间隔”。</p> 
  <pre class="language-text">+----+-------+
| Id | Score |
+----+-------+
| 1  | 3.50  |
| 2  | 3.65  |
| 3  | 4.00  |
| 4  | 3.85  |
| 5  | 4.00  |
| 6  | 3.65  |
+----+-------+
</pre> 
  <p>例如，根据上述给定的&nbsp;<code>Scores</code> 表，你的查询应该返回（按分数从高到低排列）：</p> 
  <pre class="language-text">+-------+------+
| Score | Rank |
+-------+------+
| 4.00  | 1    |
| 4.00  | 1    |
| 3.85  | 2    |
|&nbsp;3.65  | 3    |
| 3.65  | 3    |
| 3.50  | 4    |
+-------+------+
</pre> 
 </div>
</div>

---

```sh
# Write your MySQL query statement below
```