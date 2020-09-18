#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a)


b)


c)

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

