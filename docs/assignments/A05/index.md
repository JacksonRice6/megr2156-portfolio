# A5 – [Topic]

## Objective

The objective of this assignment was to create a bracket to hold a T-beam. We were given certain knowledge and with that we had to find the rest of what we needed.

## Analyze

### Stress Analysis

Firstly I had to do a stress analysis. I broke the bracket up into 5 parts, A, B, C, D, and E.

<img width="402" height="338" alt="img1" src="https://github.com/user-attachments/assets/b609f8ba-b2bf-47ed-ae9a-fd63a1802f37" />


Now I can do a stress analysis on each part. Before I do that, however, I had to determine some things first. There are a lot of assumptions made in this assignment. I picked titanium as my material. I chose 800lbf as the load. There is a load hanging from this bracket. This load is on a strap that hangs over part A's cylinder. This is a strap that has a width of .75in, and a thickness of neglibility.

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf" src="https://github.com/user-attachments/assets/01cbfb29-bedd-4088-9d29-c202e4246536" />


Starting with part A, which is a cylinder, I needed to determine its radius. For the length I assumed 1 inch, really it just needed to be bigger than the width of the strap. I wrote my knowns and unknowns and assumptions. I then drew a FBD to visualize how to force is distributed and how many forces I have. I used the equation: r = 

$$
\sqrt[3]{\frac{4Z}{\pi}}
$$

Where Z = $SF \cdot W \cdot \left(\frac{l}{2S_y}\right)$. I found r to be 0.324in. I also found the max strength where I used: $-\frac{W \cdot L}{2 \cdot Z}$. This gave me a max strength of 29962.55 psi.

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf (1)" src="https://github.com/user-attachments/assets/b5116c3e-41a6-4b26-9e0f-ca55deffa848" />

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf (2)" src="https://github.com/user-attachments/assets/6067d91c-f869-4330-98c6-f86e1bdd1eb6" />

For parts B, C, D, and E I did essentially the same thing. Assumed some dimensions and found the missing one using a stress analysis. I just used common sense for the assumptions. For B I assumed a height of .5 inches. I didn't want it too long to keep it compact and it also needed to easily fit the strap. For the lengths I knew it had to be longer than A so I just went with 1.5 inches. For the other parts I used the given dimensions of the T-Beam and knew it needed space.

<img width="664" height="311" alt="img~" src="https://github.com/user-attachments/assets/474446fa-0a95-4359-9bff-0056a3ed89a3" />

### Stiffness Analysis

This time I was given a max deflection of 0.005 inches and I used that to find the dimensions. I used primarily two dimensions: $\delta_{\text{max}} = \frac{5W \cdot L^{3} \cdot SF}{384 \cdot E \cdot I}$ , $\delta_{\text{max}} = \frac{P \cdot L \cdot SF}{E \cdot A}$.

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf (3)" src="https://github.com/user-attachments/assets/8d51942f-e0f7-4581-b24f-fe03364708f5" />

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf (4)" src="https://github.com/user-attachments/assets/ed61ed43-4e97-46c8-b034-7c0ec6006c91" />

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf (5)" src="https://github.com/user-attachments/assets/1db968a8-c556-49e1-912e-98318082b20a" />

For part A I found I then set I equal to: $\frac{\pi \cdot d^4}{64}$. I then found d to be 0.686 inches which gives a 0.343in radius. I repeated this for each part, found I then the missing dimension.

### Multiviews

<img width="1514" height="2000" alt="2026-09-14 22-11 pdf (6)" src="https://github.com/user-attachments/assets/189de34e-4d1e-458c-952e-b21e347ad4d4" />

The stiffness analysis ended up yielding much larger values, so that is the one I will go with, just to be safe.

## Decide

I decided on the material on this assignment. This impacted every single calculation and ended up being really important.

## Communicate

### Lesson Learned

#### Governing failure mode

One was really similar however, the radius. For the stiffness I got 0.343in and for the stress I got 0.324 inches. Just from this it seems that stiffness ends up giving larger dimensions, but I am sure it varies depending on several variables, so it is best to just do both tests. 

#### Error propagation

The radius of part A affected the width of part B which affected the thickness. At first I treated the radius as diameter so the width of part B was half of what it should be. Luckily I caught it when it happened but that would have affected a lot. 

#### Assumption sensitivity

As stated earlier I assumed material. This affected modulus of elasticity which affected the stiffness analysis and the strength which affected the stress analysis.

I learned how to use and compare stress and stiffness analysis and how to divide a part into different sections making it easier to manage. This will carry onto future projects.

This assignment took me 4 hours to complete.
