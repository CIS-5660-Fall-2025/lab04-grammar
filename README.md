# lab04-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## Result
### Puzzle 1
<img height="160" src="images/1-1.png"> <img height="160" src="images/1-2.png"> <img height="160" src="images/1-3.png">

Rules:
```
Premise: F
Rule 1: F=FF[+FF]F[+FF]FF+
Angle: 20
```

### Puzzle 2
<img height="160" src="images/2-1.png"> <img height="160" src="images/2-2.png"> <img height="160" src="images/2-3.png">

Rules:
```
Premise: -F
Rule 1: F=F-F+F+F-F
Angle: 90
```

### Custom plant
![](images/3-4.png)
This picture shows the l-system's generation when iteration = 8.

I divided the tree into two main components: the **trunk** and the **branches**. At the end of each trunk segment, 3 branches evenly spaced in three directions grow outwards. Each branch then generates two smaller branches. In my rules, `A` represents a trunk layer which includes 3 branches at that level. `A` repeats itself recursively at the end so that the tree can continue growing. `B` represents a branch that includes two smaller branches. It also repeats itself at the end of each smaller branch.

I applied randomization at several points within the rules to increase variation. I also utilized Houdini's convention - putting `!` before a parameter makes its thickness depend on the number of generations.

My rules are:
```
Premise: ~(5)F~(5)FA
Rule 1: A = !~(5)F~(5)F~(5)F~(5)F[+B]\(b)[+B]\(b)[+B]A
Rule 2: B = ~(20)!F[\+(c)FB][\-(c)FB]
```

Variables:
```
Angle: 75
Variable b: 120
Variable c: 15
```

Generations from different iterations:
| <img width=500px src="images/3-1.png">  | <img width=500px src="images/3-2.png"> | <img width=500px src="images/3-3.png"> | 
|:--:|:--:|:--:|
| *iteration=5* | *iteration=6* | *iteration=7* |

Generations with different seeds (iteration = 8):
| <img width=500px src="images/3-5-1.png">  | <img width=500px src="images/3-5-2.png"> | <img width=500px src="images/3-5-3.png"> | 
|:--:|:--:|:--:|
| *seed 1* | *seed 2* | *seed 3* |

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
