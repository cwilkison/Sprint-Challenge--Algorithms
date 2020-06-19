#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) This run time is O(n) because there is a linear algorithm with one loop.


b) This is a run time of O(n^2) because it contains two loops nested

c) This recurvise algorithm is also linear and runs at O(n) calls bunny ears recursively
for number of buny ears there are

## Exercise II


1) Take the total number of floors and divide it by 2

2) For example, to top floor is 50, the middle is 25 and the ground is 0

3) Drop the egg from the middle floor

  a) If the egg survives, keep top floor at 50 and move bottom from 0 to 25

  b) If the egg breaks, drop top survivable floor to 25 and keep bottom at 0

4) establish the new mid point between the top survivable and bottom survivable floor

5) continue experiment steps 3 -4 until the midpoint is equal to the highest survivable drop an egg can make

6) The run time is O(log n) because this follows a binary search procedure
