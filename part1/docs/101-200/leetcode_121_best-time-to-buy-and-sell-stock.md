# 121. [简单] 买卖股票的最佳时机

**题目链接：**[https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock)

---

<div class="content__1Y2H">
 <div class="notranslate">
  <p>给定一个数组，它的第&nbsp;<em>i</em> 个元素是一支给定股票第 <em>i</em> 天的价格。</p> 
  <p>如果你最多只允许完成一笔交易（即买入和卖出一支股票），设计一个算法来计算你所能获取的最大利润。</p> 
  <p>注意你不能在买入股票前卖出股票。</p> 
  <p><strong>示例 1:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> [7,1,5,3,6,4]
<strong>输出:</strong> 5
<strong>解释: </strong>在第 2 天（股票价格 = 1）的时候买入，在第 5 天（股票价格 = 6）的时候卖出，最大利润 = 6-1 = 5 。
     注意利润不能是 7-1 = 6, 因为卖出价格需要大于买入价格。
</pre> 
  <p><strong>示例 2:</strong></p> 
  <pre class="language-text"><strong>输入:</strong> [7,6,4,3,1]
<strong>输出:</strong> 0
<strong>解释: </strong>在这种情况下, 没有交易完成, 所以最大利润为 0。
</pre> 
 </div>
</div>

---

```java
class Solution {
    public int maxProfit(int[] prices) {
        
    }
}
```

```java
/**
 * 给定一个数组，它的第 i 个元素是一支给定股票第 i 天的价格。
 * <p>
 * 如果你最多只允许完成一笔交易（即买入和卖出一支股票一次），设计一个算法来计算你所能获取的最大利润。
 * <p>
 * 注意：你不能在买入股票前卖出股票。
 */
class Solution {
    public int maxProfit(int[] prices) {
        // 当前最小值
        int curMin = Integer.MAX_VALUE;
        int res = 0;
        for (int price : prices) {
            if (price < curMin) {
                curMin = price;
            }
            res = Math.max(res, price - curMin);
        }
        return res;
    }

//    public static void main(String[] args) {
//        int[] prices1 = {7, 1, 5, 3, 6, 4};
//        int[] prices2 = {7, 6, 4, 3, 1};
//
//        Solution1 solution = new Solution1();
//
//        System.out.println(solution.maxProfit(prices1));
//        System.out.println(solution.maxProfit(prices2));
//    }
}
```