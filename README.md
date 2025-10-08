# lab04-grammars
Let's practice using grammars! For this lab, please pull up the L-system node in Houdini.

## 1. Wheat grammar puzzle

<img height="300" alt="Wheat1" src="https://github.com/user-attachments/assets/b238b97a-a061-4b77-a520-f87f4d9a54b9" />
<img height="300" alt="Wheat2" src="https://github.com/user-attachments/assets/861661e7-b1ac-4a9c-be29-4e17152f9d07" />
<img height="300" alt="Wheat3" src="https://github.com/user-attachments/assets/2bb94b03-6b37-4748-ad76-e9348a7bbf3d" />

## 2. Square grammar puzzle
<img height="300" alt="Square1" src="https://github.com/user-attachments/assets/ab6fd8f4-cf40-4468-849f-69eb3f00c5a3" />
<img height="300" alt="Square2" src="https://github.com/user-attachments/assets/ef00745a-6709-4b9b-84f8-7ff46186d0d9" />
<img height="300" alt="Square3" src="https://github.com/user-attachments/assets/385403fd-5120-4d3f-ae10-bb474dd2037a" />

## 3. Custom plant

#### Referece image
<img height="400" alt="Leavesfinal" src="https://github.com/user-attachments/assets/14bec264-58fb-41c2-9ad6-dd69bfce3a88" />

#### Final output image
<img height="300" alt="Leavesfinal" src="https://github.com/user-attachments/assets/75c900b5-1ecf-43ce-8b00-99a48837417f" />

#### Iterations
- 2 iterations:
  - <img height="300" alt="Leaves2" src="https://github.com/user-attachments/assets/adabd94f-5b46-4a18-b176-695177990110" />
- 5 iterations:
  - <img height="300" alt="Leaves5" src="https://github.com/user-attachments/assets/689d3dc6-b2bd-4ba8-8b93-71c87cce986f" />
- 9 iterations:
  - <img height="300" alt="Leaves9" src="https://github.com/user-attachments/assets/a845a673-e291-49e4-9884-a84037b86f6f" />

The rules used to create this l system:
- Premise: Y\(70)Y (initial stem)
- Y=[\(70)&(20)X][X/(90)X] (nodes for sprouting children stems)
- X=F&(10)F&F&(5)A (nodes for sprouting leaf stems)
- A=[-&B][-&(20)b)][&B][&+\(5)b][&(10)B] (specifies how many leaf stems and in what directions)
- B=DDDDDD% (specify how many nodes for leaves)
- b=DDDDDDDD% (more nodes of leaves for variation)
- D = &(6)H[\(20)+C][/(20)-C] (draws two leaves per node, one leaf on each side)
- C=(70)O (start node for drawing an actual leaf)
The following renders out a meshed leaf:
- O=[N][M]
- N=[+(10)N{.].K.}
- M=[-(10)M{.].K.}
- K=H(0.02)H(0.05)K
