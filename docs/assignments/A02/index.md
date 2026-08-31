# A2 – Truss Stress Analysis

## Objective
The objective of this project was to design a truss able to hold a given load. We had to design the truss on paper and CAD as well as calculate the dimensions based on certain properties.

## Analyze

### The Design

[img1.pdf](https://github.com/user-attachments/files/31665845/img1.pdf)

![Design](img1.pdf)


First step was designing the truss. To do this I just made it as simple as possible. I connected each joint with straight beams, which I realized too late wasn't the most structurally sound design. I then calculated the external and internal forces for each joint. From that I found what the largest force was, just to be safe. See, in order to calculate the dimensions you have to know the force exerted. Since I picked the largest force I knew that the dimensions would work for all members.

### Finding the Area and Weight of the Beam

[img2.pdf](https://github.com/user-attachments/files/31665863/img2.pdf)


To find the area of each beam I wrote out the knowns and unknowns. Once that was done I was able to calculate the minimum cross sectional area of each beam using the properties of the material, safety factor, and load. I found the cross sectional area to be 640mm^2. At first I was going to make it a circle, but later changed it to a rectangle that was 25mmx25.6mm. Once I found that I used a simple formula to find the weight of each member using the density, length, and area. I then added each member to get the total weight of the truss which ended up being 12.979kg.

### Pins

[img3.pdf](https://github.com/user-attachments/files/31665866/img3.pdf)

[img4.pdf](https://github.com/user-attachments/files/31665867/img4.pdf)



Next were the pins. The pins were simple compared to the members. I started once again by writing out the knowns and unknowns. I did a shear stress analysis to find the most load a pin takes, I found it to be 25kN. Using that and a similar formula as before, I found the minimum cross sectional area of each pin needs to be 85.161mm^2. I made these into circles so the diameter was 10.413mm. The weight was calculated the same way and then I multiplied by 4 because there are 4 pins. The total weight of all 4 pins came out to be .067kg(~.017kg each pin).

### CAD Design

[img5.pdf](https://github.com/user-attachments/files/31665872/img5.pdf)


I needed a way to connect each member. I first came up with this square idea but realized the sharp corners would cause problems. Because of this I redesigned it to be circular, to allow for rotation.

(img6)

I designed each member separately then joined them together in an assembly file. I decided once I got to the CAD to make it a perfect square that was 28x28mm which gives a 784mm^2 area rather than a 640mm^2. This made the design easier and gave a little extra cushion.

(img7)
(img8)

I then extruded it and cut the ends off to make it rounded. After that I added the hole for the pin and cut out the connecting pieces.

(img9)

Once all assembled and material assigned the total weight was 14.6kg. The weight was slightly off. This is because the cross sectional area was more and the material chosen had a density of 7850 kg/m^3 rather than 7800 kg/m^3 because they did not offer A500 steel so I had to use AISI 4340 Steel.

(img10)

The pins were once again simple. I just made a cylinder with the appropriate dimensions. I made a custom material to assign to the pin in order to fit the given properties.



## Decide
_Which geometry did you select, and why? This is your first open design choice in the course — defend it._

## Communicate

