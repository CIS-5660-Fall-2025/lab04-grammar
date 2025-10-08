# 1. Wheat grammar puzzle

<img width="800" alt="Wheat" src="https://github.com/user-attachments/assets/e8692d73-90f4-4aba-a7cc-96a97c58f857" />

# 2. Square grammar puzzle

<img width="800" height="250" alt="Squares" src="https://github.com/user-attachments/assets/f6ce85d6-aa70-42da-836e-47438c2ebda3" />

# 3. Custom plant (Bleeding Heart)

## Reference
<img width="400" src="https://github.com/user-attachments/assets/4bb67e84-72e4-43cf-bddc-37c686541f21" />

The full plant is kind of a bush, so I just focused on making the vines and the flower.

Here are the Rules:

## Premise 

[G[-(30)H-(60)H-(60)H+(30)H+(30)H]B][/(120)G[-(30)H-(60)H-(60)H+(30)H+(30)H]B][/(240)G[-(30)H-(60)H-(60)H+(30)H+(30)H]B]

Creates 3 branches, offset by 120 degrees (evenly distributed). Then we angle it up (increasing angle makes it hang lower). We then use our branch rule, and end it with a flower (otherwise end of branch will be bare).

## Flower Rule

B=+(90)+FFFF+(180)[F+(28)F+(28)F+(28)F+(28)F+(28)F+(28)F+(28)F+(28)FFFF-(28)F-(28)-(28)-(28)-(28)-(45)FF+(60)H+(60)H+(60)FF+(30)F+(90)FH+(180)HF-(90)H+(146)F-(40)F+(70)H][F-(28)F-(28)F-(28)F-(28)F-(28)F-(28)F-(28)F-(28)FFFF+(28)F+(28)+(28)+(28)+(28)+(45)FF-(60)H-(60)H-(60)FF-(30)F-(95)FFF+(180)FFF+(95)H-(146)F+(40)F-(70)H]

This rule traces the outline of the flower. The design is slightly assymettrical, so the two capture groups are not simply reversed. We also begin by creating a stem that offsets the flower, and is influenced a little by the angle so we don't get overlap with the vine.
## Vine 

G=+[-(30)F-(60)F-(60)F+(30)F+(30)F]FFFF+FF+FF-FFF+FFF-FFF[B]G

This one is pretty simple. We offset the rotation, then create the tiny twirly vine on the top in a capture group. After that, we do some forward draws with rotations for the wavy vine, then end with a flower and a recursion.

## N = 1
<img width="400" alt="bleedingHeart" src="https://github.com/user-attachments/assets/e8402ffc-9131-4b6e-9a4c-8811ae79d8ea" />

## N = 2
<img width="400" alt="bleedingHeart2" src="https://github.com/user-attachments/assets/ab13b3af-040d-4a93-8935-f3b7c238c145" />

## N = 3
<img width="400" alt="bleedingHeart3" src="https://github.com/user-attachments/assets/fbf8fed0-fc37-45ba-8d21-63d690f9a987" />
