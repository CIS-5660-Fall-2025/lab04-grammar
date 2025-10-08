# lab04-grammars

Name: Tianhong Zhou

## 1. Wheat grammar puzzle

![](imgs/wheat_puzzle.png)

## 2. Square grammar puzzle

![](imgs/square_puzzle.png)

## 3. Custom plant

Components and Intent

1. **Trunk (`A`)**  
   `A = F[^+FB][\-B][&-FFB]`  
   - `F` advances the central axis (trunk).  
   - `[^+FB]` spawns a branch cluster: first **pitch up** (`^`), then **yaw left** (`+`), creating an upward/left lateral that continues into `F B`.  
   - `[\-B]` applies a **roll left** (`\`) and **yaw right** (`-`) before growing `B`, producing a branch with a distinct banked orientation.  
   - `[&-FFB]` **pitches down** (`&`), yaws right (`-`), then advances twice before `B`, yielding a lower, outward-reaching scaffold limb.  
   Together, these three bracketed branches around each trunk step create an asymmetric, spreading crown typical of oak.

2. **Secondary Branching (`B`)**  
   `B = F[^-FC][&+C][/+C][\-C]`  
   - `F` advances to set internode length.  
   - `[^-FC]` pitches up and yaws right into `F C` - an ascending lateral that continues to `C`.  
   - `[&+C]` pitches down and yaws left - a descending/side limb.  
   - `[/+C]` rolls right and yaws left - banking changes the azimuth spread.  
   - `[\-C]` rolls left and yaws right - creating another azimuth.  
   Collectively, `B` fans children into multiple azimuths with distinct pitch, forming the oak's rounded, horizontally spread canopy.

3. **Twig Level (`C`)**  
   `C = F[^+B][\-FB][&-B]`  
   - `F` advances slightly.  
   - `[^+B]` (up + left) and `[\-FB]` (roll left, yaw right then forward) and `[&-B]` (down + right) generate final-order branching back into `B`.  
   This closes the hierarchy (C->B->C...), yielding a dense, multi-order branching that still respects the 3D variation.

![](imgs/custom.png)

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
