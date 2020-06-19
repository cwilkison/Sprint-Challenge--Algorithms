# Analysis of Algorithms

## Exercise I

Give an analysis of the running time of each snippet of
pseudocode with respect to the input size n of each of the following:

```python
a)  a = 0
    while (a < n * n * n):
      a = a + n * n
```


```
b)  sum = 0
    for i in range(n):
      j = 1
      while j < n:
        j *= 2
        sum += 1
```

```
c)  def bunnyEars(bunnies):
      if bunnies == 0:
        return 0

      return 2 + bunnyEars(bunnies-1)
```

## Exercise II

Suppose that you have an n-story building and plenty of eggs. Suppose also that an egg gets broken if it is thrown off floor f or higher, and doesn't get broken if dropped off a floor less than floor f. Devise a strategy to determine the value of f such that the number of dropped + broken eggs is minimized.

Write out your proposed algorithm in plain English or pseudocode AND give the runtime complexity of your solution.


1) Take the total number of floors and divide it by 2

2) For example, to top floor is 50, the middle is 25 and the ground is 0

3) Drop the egg from the middle floor

  a) If the egg survives, keep top floor at 50 and move bottom from 0 to 25

  b) If the egg breaks, drop top survivable floor to 25 and keep bottom at 0

4) establish the new mid point between the top survivable and bottom survivable floor

5) continue experiment steps 3 - 4 until the midpoint is equal to the highest survivable drop an egg can make

6) The run time is O(log n) because this follows a binary search procedure

