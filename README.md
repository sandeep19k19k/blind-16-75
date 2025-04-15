# blind-16-75
Climbing stairs


This is a classical Dynamic programming problem.

kind of similar to fibonacci problem.

 Ways(n) = Ways(n-1) + Ways(n-2)


Basically, you can get the idea by analyzing the examples.

no.of steps= 1 2 3 4 5 6 

no.of ways= 1 2 3 5 8 13

And the pattern is clearly similar to fibonacci, except the initial 2 values.


i.e we are trying to make use of the already calculated values and find the optimum solution as we traverse along the problem, without calculating the same results again and again.

 ( in recursion, recalculation happens , where time complexity is 

O(2^n) --->exponential

 space complexity : O(n) stack space. i.e function is called for each of the n-1 values . Hence ,not optimal ).

Here one more key thing to observe is the fact that , we don't need to store all the ways associated with n-1 steps.

i.e we don't a list ( consumes extra space O(n)).

we just need to keep a track of no.of ways associated with n-1 and n-2.


Time complexity : O(n) (DP is lovely )

Space complexity : O(1)
