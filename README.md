# lab04-grammars

Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle

Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

![p1-1.png](img/p1-1.png)

![p1-2.png](img/p1-2.png)

![p1-3.png](img/p1-3.png)

## 2. Square grammar puzzle

How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

![p2-1.png](img/p2-1.png)

![p2-2.png](img/p2-2.png)

![p2-3.png](img/p2-3.png)

## 3. Custom plant

<img title="" src="img/bamboo.png" alt="bamboo.png" width="248">

![p3-4.png](img/p3-4.png)

Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

### **Axiom `[+X][-X][X]`**

The brackets `[` and `]` save and restore the current turtle state (position and orientation).  
The `+` turns the heading to the left by the specified angle, and `-` turns it to the right.  
Together, `[+X][-X][X]` generates three main stems from the same base point — one turning left, one right, and one growing straight ahead.

---

### **Rule 1 `X = F[+X][-\X]&F[+\X][-X]FX`**

`F` moves the turtle forward, drawing one segment of the stem.  
`[+X]` creates a branch rotated left, while `[-\X]` creates a branch rotated right and rolled left (`\`) so that branches are distributed around the axis rather than lying in a single plane.  
`&` pitches the heading downward, making the next branches slightly droop.  
The following `F` moves forward again, `[+\X][-X]` generates another left–right pair of branches, then `F` advances once more before `X` recursively calls itself to continue growth.  

---

### **Rule 2 `F = FF`**

`F` means “move forward.”  
Replacing it with `FF` doubles the forward step distance, effectively elongating each internode and producing taller, more slender stems characteristic of bamboo-like growth.

![p3-1.png](img/p3-1.png)

![p3-2.png](img/p3-2.png)

![p3-3.png](img/p3-3.png)

## Submission

- Create a pull request against this repository
- In your readme, list your solutions and format your README nicely
- Profit
