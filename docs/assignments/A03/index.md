# A3 – [Topic]

## Objective

For this assignment I was tasked with designing a cylindrical beam that would be pulled from one side. I had to find the length needed given deflection, material, and force, I picked the area.

## Analyze
### Finding the Length

(img1)

First things first I had to find the length. I was given the max deflection of 0.009" a force of 500lbs and a modulus of elasticity of 11.5x10^6psi. I was allowed to pick the area I desired. At first I gave the beam a 2" diameter which was an area of 3.14in^2. However, this made the length 650.3". This was obviously way too long so I needed to decrease the area. I ended up going with a 0.5" diameter which was an area of 0.196in^2. This gave me a new length of 40.644", which was much more managable.

### CAD

(img2)

Next step was going into Solidworks. The first thing I did was set up my parametrics. These were things like E and F and all that, this way I could easily change any dimensions I needed to once I built the beam. I also set length equal to E x A x deflection / force. So Solidworks determines the length for me, even though I already found it.

(img3)

Once the beam was constructed I did an FEA. This simulates force on the beam and gives you the results of things like displacement and stress. What I was looking for was displacement, stress, and the safety factor. The deflection was 0.00904in and the max stress was......

### Calculated vs Computer

Solidworks gave me a displacement of 0.00904 inches while I calculate 0.009 inches. These values are very very close, just 4/100 of a thousandth of an inch different. This makes sense because in my calculations I said deflection was equal to 0.009 which gave me the length. So then it was just reliant on math. Mathematically speaking, they had to be the same.


## Decide


## Communicate

