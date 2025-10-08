# lab04-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output. Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

### Solution

<img width="808" height="299" alt="Screenshot 2025-10-08 105948" src="https://github.com/user-attachments/assets/96d3b2a4-e830-4dad-9b23-5c58b3bb30a1" />


## 2. Square grammar puzzle
How about this one? Take a screenshot of your rules.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

### Solution

<img width="798" height="219" alt="Screenshot 2025-10-08 110937" src="https://github.com/user-attachments/assets/79eeef7a-cea7-41c1-893a-be18f5a49de6" />


## 3. Custom plant
Choose a plant in the world. Working off a reference, design a grammar that mimics the structure of that plant. Unlike our simple puzzles, please use multiple rules for greater complexity. Think carefully about the structure of your grammar! EXPLAIN the structure of your plant in the README. What are the components? What do each of the rules do? Be sure to also include images of a few iterations of your output plant. 

### Submission
<img width="659" height="635" alt="Screenshot 2025-10-08 150942" src="https://github.com/user-attachments/assets/318e4e05-b160-4629-9617-18c9e64f92c3" />
<img width="557" height="699" alt="Screenshot 2025-10-08 150905" src="https://github.com/user-attachments/assets/918b5fe1-24de-41e0-82ca-5a4ebe0f814e" />

I tried to replicate the structure of a fern. The first grammar rule defines the recursion of A, which extends the length of the fern and curls it inwards. The second rule creates the offshoots from the fern's center, oriented towards the end of the plant. The third rule creates further offshoots from the first offshoots to give the fern its leaves. Aside from the first rule extending the end of the plant with offshoots every iteration, recursion is not present for the other rules, since a fern has little recursion and is more orderly in structure.

<img width="614" height="183" alt="Screenshot 2025-10-08 150959" src="https://github.com/user-attachments/assets/b68c3866-2333-49f8-bcc3-eef5cfaf9a6a" />

