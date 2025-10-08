# lab04-grammars

In this lab we practiced using L_system nodes in houdini by designing grammars to replicate certain outputs.

## 1. Wheat grammar puzzle

Reference

|<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949661-a3a0e1f7-7d68-4b9e-8384-d9991e1e9fd2.png">|<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949853-cf2306b3-3537-4c24-91b5-0a3083bc87c0.png">|<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949859-5e432b4b-f18d-48b5-a9e9-8d7dba255955.png">|
|:--:|:--:|:--:|
|*Reference n = 1*|*Reference n = 2*|*Reference n = 3*|

Solution:
* Premise: F
* Rule: F = F=FF[+FF]F[+FF]FF+

|![](img/wheat1.png)|![](img/wheat2.png)|![](img/wheat3.png)|
|:--:|:--:|:--:|
|*Solution n = 1*|*Solution n = 2*|*Solution n = 3*|

## 2. Square grammar puzzle

Reference
|<img width="200" alt="square1" src="https://user-images.githubusercontent.com/1758825/193949895-87cdfb43-da7c-4867-ab1b-107e1ba9d2a7.png">|<img width="200" alt="square2" src="https://user-images.githubusercontent.com/1758825/193949904-a9cdfe0f-319e-4ca8-9935-dd338217a7cf.png">|<img width="200" alt="square3" src="https://user-images.githubusercontent.com/1758825/193949910-928e5993-ce26-4681-80f8-ffeb54be4dcf.png">|
|:--:|:--:|:--:|
|*Reference n = 1*|*Reference n = 2*|*Reference n = 3*|

Solution:
* Premise: -F
* Rule: F=F-F+F+F-F

|![](img/Square1.png)|![](img/Square2.png)|![](img/Square3.png)|
|:--:|:--:|:--:|
|*Solution n = 1*|*Solution n = 2*|*Solution n = 3*|

## 3. Custom plant

For the last part, I chose a custom plant and designed a grammar to mimic it's structure. Here's some reference images of oak trees:

|![](img/oakTree1.webp)|![](img/oakTree2.jpg)|![](img/oakTree3.jpg)|
|:--:|:--:|:--:|
||||

And here are some pictures of my L system

* Premise: X
* Rule 1: (Trunk branching) X = F [+Y] [-Y]
* Rule 2: Y = FFBF
* Rule 3: (Fan branching shape) B =  [ /(0) &(35) F(0.20) X] [ /(36) &(35) F(0.20) X]
     [ /(72) &(35) F(0.20) X] [ /(108) &(35) F(0.20) X]
     [ /(144) &(35) F(0.20) X] [ /(180) &(35) F(0.20) X]
     [ /(216) &(35) F(0.20) X] [ /(252) &(35) F(0.20) X]
     [ /(288) &(35) F(0.20) X] [ /(324) &(35) F(0.20) X]

|![](img/3tree.png)|![](img/5tree.png)|![](img/7tree.png)|
|:--:|:--:|:--:|
|*Tree n = 3*|*Tree n = 5*|*Tree = 7*|

|![](img/9tree1.png)|
|:--:|
|*Tree n = 9*|
