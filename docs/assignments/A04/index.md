# A4 – [Topic]

## Objective

For this assignment I had to design a motor mount for a motor. This had to support a force of 300N and hang on a surface. I was given the model of the motor along with its dimensions to help me with the design.

## Analyze

#### Feature 1

(img1)

This is the part of the motor mount that holds the motor. As normal I listed my knowns and unknowns. Once I did that I set up two different equations, both with the same goal, to find the unknown dimension. Essentially whichever equation gave me the bigger value, is the value I would pick. This is because this just adds an extra bit of cushion. You know the minimum height you need for one equation is less than the minimum height for the other, so go with the other one. For this feature I picked all the other dimensions. To do this I used the dimensions of the motor given. The motor had a diameter of 28mm, so I made a hole with a 30mm diameter to give a little wiggle room and gave it a depth of 4mm to somewhat secure it. I then repeated this process for similar features of the motor. The holes are design for M3 screws.

#### Feature 2

(img2)

This feature attaches to the wall. This had a similar process. I started with my knowns and unknowns and started finding the thickness of this feature which I named h2. I set up the max deflection and max stress equations. The max deflection gave me 26.78mm which was the bigger of the two values. The holes on the back are designed for M6 screws.

(img)

#### CAD

<img width="781" height="351" alt="Parametrics" src="https://github.com/user-attachments/assets/3d22ca3f-0438-492f-8369-2014ed931d29" />


To design this in Solidworks I started with the parametrics. This will help me later.

<img width="440" height="407" alt="Basis" src="https://github.com/user-attachments/assets/f2ba8014-3875-416f-8a14-d51d87fb698f" />


I then sketched out a basic shape and extruded it by the base.

<img width="820" height="721" alt="Pattern" src="https://github.com/user-attachments/assets/9a32097e-4fb1-4451-9c9d-388c4d543413" />

<img width="469" height="341" alt="M6Hole" src="https://github.com/user-attachments/assets/96dbde03-c45b-4b4e-915a-e37c5ba5fb1b" />


Then I put a hole for the screw on feature 2 and used a linear pattern to make 4 of them.

<img width="1032" height="693" alt="Circles" src="https://github.com/user-attachments/assets/6ff64723-4304-4475-9040-458327f89111" />


Then I made the holes on feature 1. I put the circles to size and then put the screw holes and used a circular pattern array to put 4 of them symmetrically. After that I just did a cut extrude on each circle to the desired depth.

<img width="444" height="392" alt="Hole1" src="https://github.com/user-attachments/assets/04117ed7-1d28-437f-8d9d-68ed4f96bcaa" />
<img width="470" height="374" alt="Hole2" src="https://github.com/user-attachments/assets/38dacf4d-3d1c-4abf-9d0a-cf91f5c2e50c" />
<img width="439" height="354" alt="Hole3" src="https://github.com/user-attachments/assets/aa83218e-6c46-4114-a1a5-dc4711f26ade" />



## Decide

I decided in this project to makes these depth holes for the motor. Some may have seemed unnecessary, like the biggest hole, but it was just extra security and personally I am really happy with it.

## Communicate

In this project I learned how to find minimum thickness(or any dimension) for a part by using different equations. It may not always be the stress or deflection, but it is really useful to know, and I know it will prove very helpful in the future. This assignment took me 4 hours.

#### CAD Files

[Mount.zip](https://github.com/user-attachments/files/32219831/Mount.zip)
