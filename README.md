# lab04-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.
<img width="992" height="870" alt="Screenshot 2025-10-08 104748" src="https://github.com/user-attachments/assets/aeacfd1a-919b-4969-a288-c0111159df0d" />
1:

Premise:
`F`

Rule:
`F=FF[-FF]F[-FF]FF-`

<img width="992" height="870" alt="Screenshot 2025-10-08 105054" src="https://github.com/user-attachments/assets/3a0e073d-3469-4236-9121-e8cd0a17101e" />
2:

Premise `+F`

Rule:`F=F+F-F-F+F`

<img width="992" height="870" alt="Screenshot 2025-10-08 115635" src="https://github.com/user-attachments/assets/96b9d597-71ba-4880-82b8-63ecd402f136" />
<img width="992" height="870" alt="Screenshot 2025-10-08 115645" src="https://github.com/user-attachments/assets/ac0866ce-cfce-4ed2-9819-6ae37d98cdcd" />

3:

Premise: `#(0.6)A`

Rules:

`A=FF[-(90)B]+F-[+(88)B]F+F[+(60)B][-(90)B]-FA:0.65`

`B=F(0.08)CFEB:0.8`

`C=[#(-0.5)[-(60)F][+(60)F]]:0.7`

`C=[-(23)B][+(23)B]:0.1`

`B=[#(-0.5)F]:0.12`

`A=FF[-(90)B]-F+[+(88)B]F-F[+(100)B][-(90)B]+FA`

`C=[+(5)B]`

`B=F(0.06)ED:0.05`

`D=F(0.08)ED:0.8`

`D=[#(-0.5)F]`

`E=[#(-0.5)[-(60)F][+(60)F]]`

`B=[-(5)B]:0.01`

`B=[+(5)B]`

TODO finish writing up explanation

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
