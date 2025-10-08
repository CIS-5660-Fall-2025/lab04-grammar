# Results

## 1. Wheat grammer puzzle
![](scrPuzzle1.png)

## 2. Square grammer puzzle
![](scrPuzzle2.png)

## 3. Custom plant
I tried to design my custom plant with this crimson fractal image as a reference.
![](ref.jpg)
### Results
![](scrPuzzle3_n4.png)

4 Iterations

![](scrPuzzle3_n7.png)

7 Iterations

![](scrPuzzle3_n11.png)

11 Iterations

### Rules
![](scrPuzzle3_rules.png) 

The rules above drive the plant.  The premise spawns two of the long leaves.  ``C`` is a line with a branch, denoted with ``A``, coming off of the upper part.  The most important part of ``A`` that makes it a branch is ``[&A][^A]``, this tilts the L-System turtle in one direction, creates another branch, then tilts the turtle in the opposite direction and creates another branch.  This results in branches that branch into more branches on additional recursions.  
The ``B`` at the end of ``C=FFAFB`` expands into another ``FFAFB``, so each recursion, our leaf will get longer with the branches on the end having less recursions.
The ``/(10)`` in ``A =`` results in a progressive twist of the leaves.  ``+(5)`` in ``B =`` results in a progressive bend of the leaves.  The ``"`` in ``A =`` decreases the length of the lines on deeper recursions on the leaves.

---

# lab03-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

## Submission
- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
