#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)
```
a = 0 
  while (a < n * n * n):
    a = a + n * n
```
This will be O(n) because the while loop will repeat n times, so the higher the value of n, the longer it will take. Also it has since it has a 1:1 relation (n:n), the slope of this will be exactly 45 degree which is the cut off for O(n) and start of O(n^2). 

b)
```
sum = 0
  for i in range(n):
    j = 1
    while j < n: 
      j *= 2
      sum += 1
```
This will be O(n(log n)) sine the for loop will be O(n) and the while loop will be O(log n). The for loop does not have a break so it will go trough the whole range. The while loop will start exiting later and later the higher the value of n is. 

c)
```
def bunnyEars(bunnies):
  if bunnies == 0:
    return 0

  return 2 + bunnyEars(bunnies-1)
```
This is not an efficient function since it could have been returned with a calculation of 2*n which would have been O(1). Because it is recursive it will have to call the function n times (n being the value of bunnies) so it will be O(n).

## Exercise II
- define a function
- calculate the mid floor of building (n//2) --> O(1)
- if mid is equal to f --> O(1)
    - return f
- drop egg from mid --> O(log(n))
    - if egg breaks
        - recursive of this time all floors below the mid  
    - if egg does not break
        - recursive of this time all floors above the mid

The runtime complexity of this will be like a binary search and will be O(log(n)). This proposed algorithm will minimize the "dropped + broken eggs" if we assume that f is a random number and not always on the lower levels.

