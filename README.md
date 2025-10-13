# lab04-grammars
A practice of using L-system grammars in Houdini.

## 1. Wheat grammar puzzle
Look at these iterations (n = 1, 2, 3) of a one-rule grammar. Using the built in symbols in Houdini, design a grammar that produces this output.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">

My solution:\
<img width="300" src="./1.0.png">

Result images:\
<img width="400" src="./1.1.png">\
<img width="400" src="./1.2.png">\
<img width="400" src="./1.3.png">

## 2. Square grammar puzzle
Recreate these ones as well.\
<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">
<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">
<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">

My solution:\
<img width="300" src="./2.0.png">

Result images:\
<img width="400" src="./2.1.png">\
<img width="400" src="./2.2.png">\
<img width="400" src="./2.3.png">

## 3. Custom plant
My system:\
<img width="300" src="./3.0.png">\
The first 3 rules are for the trunk A:
  1. With a 45% chance, grow forward, narrow the trunk, then create two angled trunks (one bends upward with a roll, the other downward with an opposite roll). At the end, extend the trunk again.
  2. With a 35% chance, grow forward, narrow the trunk, then split into three: one rolls right, one pitches downward by b degree, and one rolls left.
  3. With a 20% chance, extend the trunk and attach a branch B at the end.

The other 2 rules are for the branch B:
  1. With a 60% chance, grow forward in a shorter distance, narrow the branch, then fork into two side twigs at plus and minus c degrees.
  2. With a 40% chance, grow forward in a shorter distance, narrow the branch, then split upward and downward around the vertical axis by c degrees.




Result images:\
<img width="400" src="./3.1.png">\
<img width="400" src="./3.2.png">\
<img width="400" src="./3.3.png">
