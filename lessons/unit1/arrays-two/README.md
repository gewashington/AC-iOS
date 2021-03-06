### Arrays - Day 2

### Review:


```swift
let myArr = [1,5,2,3,194,-32]
```

1. print out all the numbers in the array
2. print out the length of the array
3. print out the last element in the array
4. print out the first element in the array
5. print out the sum of the array


### Arrays review

[https://www.weheartswift.com/arrays/](https://www.weheartswift.com/arrays/)


### 16. Arrays can be multidimensional

```swift
let theMatrix = [[1, 2, 3],
                 [4, 5, 6],
                 [7, 8, 9]]

```

We are not limited to one dimension when creating arrays.  Arrays have to take one of the same type, but that type can be another array.  When you have an array of arrays, we call that a 2-dimensional array.  This is because it has both a width (the size of each array) and a height (the total number of arrays).

We can access whole arrays by subscripting the original array:

```
let firstArr = theMatrix[0]
```

We can access individual elements by subscripting the array we get from that

```
let firstElementInFirstArr = firstArr[0]
```


We can combine both of these lines together in a single expression:

```
let firstElementInFirstArr = theMatrix[0][0]
```

Conceptually, the first index corresponds with the *row* and the second index corresponds with the *column*


**Practice**:  Print out the element in each corner, then print out the element in the middle.

### 17. Building Arrays

We can use the Array Constructor methods to create new instances of Arrays.

```
//Array(repeating: <Value>, count: <Int>)
let newArr = Array(repeating: 5, count: 2)
```

**Practice:** 

1. Make an array containing 200 copies of the number 9
2. Make an array containing 20 copies of the string "Hello"
3. Make an array of 30 optional Ints set to nil
4. Make a 2-dimensional 5 x 5 array of Ints all set to 0


### 18. Solving problems with multidimensional arrays

1. Given a square array, print out all elements
2. Given a square array, print out the difference of the two diagonals
3. Given a square array, print out the sum of the border
4. Given a square array, print out the sum of all elements in odd numbered columns
5. Given a rectangular array, print out the sum of all elements in even numbered columns


# In depth matrix problems

### Tic-Tac-Toe
Given a tic tac toe board, determine if a player has won or if it's a cat's game.

```
let TTTboard = 
[["X", "X", "X"],
["O", "O", "X"],
["X", "O", "O"]]
```



### Sudoku Solution Checker
Given a Sudoku board, determine if the board is valid.

The rules can be found [here](http://sudoku.com.au/TheRules.aspx)

```swift
let validSudokuBoard = 
[[1,5,2,4,6,9,3,7,8],
[7,8,9,2,1,3,4,5,6],
[4,3,6,5,8,7,2,9,1],
[6,1,3,8,7,2,5,4,9],
[9,7,4,1,5,6,8,2,3],
[8,2,5,9,3,4,1,6,7],
[5,6,7,3,4,8,9,1,2],
[2,4,8,6,9,1,7,3,5],
[3,9,1,7,2,5,6,8,4]]
```
