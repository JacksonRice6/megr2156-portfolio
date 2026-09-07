# A3 – [Topic]

## Objective

For this assignment I was tasked with designing a cylindrical beam that would be pulled from one side. I had to find the length needed given deflection, material, and force, I picked the area.

## Analyze
### Finding the Length

<img width="1920" height="1080" alt="Untitled design" src="https://github.com/user-attachments/assets/4d492310-a87c-4500-8b95-9fbca67d153d" />


First things first I had to find the length. I was given the max deflection of 0.009" a force of 500lbs and a modulus of elasticity of 11.5x10^6psi. I was allowed to pick the area I desired. At first I gave the beam a 2" diameter which was an area of 3.14in^2. However, this made the length 650.3". This was obviously way too long so I needed to decrease the area. I ended up going with a 0.5" diameter which was an area of 0.196in^2. This gave me a new length of 40.644", which was much more managable.

### CAD

<img width="794" height="325" alt="Parametrics" src="https://github.com/user-attachments/assets/74b326eb-69f2-47b7-83c3-2f5ef70d0207" />
<img width="221" height="111" alt="Length" src="https://github.com/user-attachments/assets/445a8103-daaf-4cde-b64c-426c0954c6a3" />


Next step was going into Solidworks. The first thing I did was set up my parametrics. These were things like E and F and all that, this way I could easily change any dimensions I needed to once I built the beam. I also set length equal to E x A x deflection / force. So Solidworks determines the length for me, even though I already found it.

<img width="541" height="480" alt="Fixed Geometry" src="https://github.com/user-attachments/assets/8963f04a-2afd-4727-94f7-90a5b4e4abe9" />


Once the beam was constructed I did an FEA. This simulates force on the beam and gives you the results of things like displacement and stress. What I was looking for was displacement, stress, and the safety factor. The deflection was 0.00904in and the max stress was 2.652 ksi. This is far less that aluminum's strength(40ksi).

<img width="1437" height="621" alt="VonMisses" src="https://github.com/user-attachments/assets/9570812f-013d-45ef-b782-698318043b40" />

<img width="1447" height="635" alt="Deflection" src="https://github.com/user-attachments/assets/32523fc9-c290-4d7e-96a4-f7ce8d5db2c4" />

<img width="1547" height="665" alt="SF" src="https://github.com/user-attachments/assets/bacccf35-82a1-4db1-ad62-1b7aebc1dccf" />




### Calculated vs Computer

Solidworks gave me a displacement of 0.00904 inches while I calculate 0.009 inches. These values are very very close, just 4/100 of a thousandth of an inch different. This makes sense because in my calculations I said deflection was equal to 0.009 which gave me the length. So then it was just reliant on math. Mathematically speaking, they had to be the same. I would trust the math more, simply because math is never wrong. While this does allow for human error, so does designing it with CAD.

### Pin Hole

For the pin hole I picked a diameter of 0.1 inches. My nominal stress was 2.652ksi, once you multiply that by the Kt value of 2.51 you get 6.656ksi. This would be the maximum stress at the pin hole. My safety factor was 14.57 so this falls well within since the safety factor is over 6 times as much as the stress concentration factor.


## Decide

In this project I decided to use the 500lb force. The assignment gave us a range but I picked the largest load that way I knew my beam was as strong as it could be for this assignment.


## Communicate

In this assignment I learned about the stress concentration factor. This is basically the ratio of the max stress to the nominal stress. It essentially tells you how stressed a part of your object is. It is very helpful for troubleshooting and making sure your part will hold. This assignment took me 2 hours.

### CAD Files


