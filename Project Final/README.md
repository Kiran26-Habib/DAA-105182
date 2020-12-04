# DAA-105182 Fall 2020: Course Repository #
### Project Members ###
StdID | Name
------------ | -------------
**63022** | **Kiran Habib**
**62354** | **Sehar Saleem**
**62621** | **Ali Hunain**

## Backtracking ##

### N Queen Problem Using Backtracking Algorithm###
The thought is to put queen individually in various segments, beginning from the furthest left section. At the point when we place a queen in a section, we check for conflicts with effectively positioned queen. In the current section, in the event that we discover a line for which there is no conflict, we mark this line and segment as a component of the arrangement. In the event that we don't discover such a line because of conflicts, at that point we backtrack and return bogus.

### Complexity ###
Number of possible arrangements of N Queens on N x N chessboard is  N! , given you are skipping row or column, already having a queen placed.
So average and worst case complexity of the solution is  O(N!).

### Idea Of The Algorithm ###
Backtracking is an algorithmic-procedure for tackling issues recursively by attempting to manufacture an answer gradually, each piece in turn, eliminating those arrangements that neglect to fulfill the correct arrangement.

## Bruteforce ##

### N Queen Problem Using Bruteforce Algorithm###
The way that the quantity of queens is equivalent to the quantity of spaces on the chessboard gives us an unmistakable favorable position. Since there are just n lines and n queens, it follows that there will be actually one queens on each line in a substantial arrangement. On the off chance that there were two queens on a column, they would be undermining one another, and we were unable to deliver a legitimate arrangement. In the event that there were any column unfilled, it would follow that we would need to fit all n queens into the leftover (n — 1) lines, which would mean two queens would be compelled to get serious about a line, which they can't do. It follows in this way that we can't have a legitimate arrangement with any vacant lines (the equivalent is valid for segments, obviously, so don't hesitate to peruse the accompanying thinking and intellectually switch 'line' with 'segment', on the off chance that you are so disposed).

### Complexity ###
The worst case “brute force” solution for the N-queens puzzle has an O(n^n) time complexity. This means it will look through every position on an NxN board, N times, for N queens. It is by far the slowest and most impractical method

### Idea Of The Algorithm ###
Yet, subsequent to "constraining" the calculation to put just one sovereign on each line and one on every segment the quantity of posible legitimate positions diminishes to N! (N!=123....*(N-1)*N). Utilizing this calculation we can found an answer for bigger table sizes contrasted with the past technique (like N=17).I won't present a genuine savage power calculation here on the grounds that it isn't handy (has exremely low speed because of the colossal measure of assets figurings required).


## Dynamic Programming ##

### N Queen Problem Using Dynamic Programming###

A connected issue is the proper n-queen problem. This issue is indistinguishable from the (normal) n-queen problem, then again, actually all diagonals are of length n and wrap as though the chessboard were on a torus. On the off chance that we signify the quantity of answers for the toroid issue as T(n), clearly T(n) < Q(n). In this paper we portray a basic calculation for registering Q(n) or T(n) in time O(f(n>8">, where f(n) is a low-request polynomial. The calculation depends on unique programming. It is an extraordinary instance of a methodology created in , which sees certain hunt issues as whole number direct programming issues and illuminates them through polynomial duplication.


### Complexity ###
Total time complexity: Ο(n^2 f(n) 2^(6n-2))
	During each iteration, we decrease the number of swaps by at least 1
	During each iteration, we consider 𝑛^2  pairs of queens
	Maximum steps to find the solution: 𝑛^3
	Experimental results show an average of Ο(𝑛 log(𝑛)) steps, even if multiple initial positions are needed
### Idea Of The Algorithm###
1. [Compaction] If (S U T, j) E QUEUE for some j, supplant j by I + j. 3.2 [Creation] Otherwise, add (S U T, i> to QUEUE. 4) [Termination] If an unexamined square remaining parts, go to step . 

2. Something else, end. decide the quantity of arrangements from QUEUE. To begin with, characterize A4 to be the arrangement of 2n lines that are At the finish of this calculation we can without much of a stretch.

### Analysis On The Algorithms ###
On large datasets best solution is dynamic programming it can work efficiently with the large dataset it gives best cmplexity. After DP backtracking has an average complexity with the large dataset. Worst case complexity can be given by Brute force with the large datset.
