---
layout: post
title:  "Algo Day 55"
date:   2023-02-19 21:01:00 -0000
categories: [Algorithm,Dynamic Programming]
---

<div class="post-categories">
  Categories:
  {% if post %}
    {% assign categories = post.categories %}
  {% else %}
    {% assign categories = page.categories %}
  {% endif %}
  {% for category in categories %}
    {% if categories[-1] == category %}
        <a href="{{site.baseurl}}/categories/#{{category|slugize}}">{{category}}</a>
    {% else %}
        <a href="{{site.baseurl}}/categories/#{{category|slugize}}">{{category}},</a>
    {% endif %}
  {% unless forloop.last %}&nbsp;{% endunless %}
  {% endfor %}
</div>

&nbsp;


### Problem 1:

[309. Best Time to Buy and Sell Stock with Cooldown](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/)

* First Thought:

  1. NA

&nbsp;

* Thoughts After Looking At The Solution:

  1. Five states.

&nbsp;

* Difficulties Encountered:

  1. Hard to distingush states.

&nbsp;

* Conclusion:

Solution:
  {% highlight python %}
    class Solution:
        def maxProfit(self, prices: List[int]) -> int:
            dp = [[0 for _ in range(4)] for _ in range(len(prices))]
            dp[0][0] = -prices[0]
            for i in range(1, len(prices)):
                dp[i][0] = max(dp[i-1][0], dp[i-1][1] - prices[i], dp[i-1][3] - prices[i])
                dp[i][1] = max(dp[i-1][1], dp[i-1][3])
                dp[i][2] = dp[i-1][0] + prices[i]
                dp[i][3] = dp[i-1][2]
            return max(dp[-1])
  {% endhighlight %}


&nbsp;


### Problem 2:

[714. Best Time to Buy and Sell Stock with Transaction Fee](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-transaction-fee/)

* First Thought:

  1. Add a transaction fee to each transaction.

&nbsp;

* Thoughts After Looking At The Solution:

  1. NA

&nbsp;

* Difficulties Encountered:

  1. NA

&nbsp;

* Conclusion:

Solution:
  {% highlight python %}
    class Solution:
        def maxProfit(self, prices: List[int], fee: int) -> int:
            dp = [[0 for _ in range(2)] for _ in range(len(prices))]
            dp[0][0] = -prices[0]
            for i in range(1, len(prices)):
                dp[i][0] = max(dp[i-1][0], dp[i-1][1] - prices[i])
                dp[i][1] = max(dp[i-1][1], dp[i-1][0] + prices[i] - fee)
            return dp[-1][-1]
  {% endhighlight %}


&nbsp;