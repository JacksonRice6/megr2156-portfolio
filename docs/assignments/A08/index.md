# A8 – Gears

## Objective
The objective of this assignment was to design and model a gear box to house two gears with their shafts. I had to calculate the diameter of the shafts and other dimensions then make engineering decisions in the design to get a functioning gear box.

## Analyze
### The Shafts

<img width="2448" height="793" alt="2026-10-16 18-34 pdf" src="https://github.com/user-attachments/assets/e45f0eba-3d08-4bef-a45f-770e21e650ba" />

The first step was the shafts. I needed to calculate the max stress of each shaft and make sure it fell within the parameters. I first started with my knowns and unknowns then drew a FBD. I had to do two separate calculations, one for the input shaft and one for the output. I chose each shaft length to be one inch knowing I could change it later if need be. I found that each given diameter was sufficient.

### Journal Bearings

<img width="2448" height="793" alt="2026-10-16 18-34 pdf (1)" src="https://github.com/user-attachments/assets/ec2c92a0-dc0d-4a20-bbaf-d7028284c60d" />

The next step was the journal bearings. These are basically oily sleeves for the shafts to spin in. I had to find a material for this shaft since it would be experience high pressure and high speeds. To do this I found the max pressure and max velocity, 11.26psi and 95.99 ft/min respectively, which gave a max PV of 1080.85 psi*ft/min. I then used this information on a table to find the right material. I found the best material to be acetal. 

<img width="2448" height="793" alt="2026-10-16 18-34 pdf (2)" src="https://github.com/user-attachments/assets/52ba61d8-607b-4767-8e70-d65f85814ca6" />


Last step was finding the thickness of the journal bearings which I found to be .000937 inches, very thin.

### Sketch

<img width="2448" height="793" alt="2026-10-16 18-34 pdf (3)" src="https://github.com/user-attachments/assets/177627c8-9137-4600-8bac-ebe4fd0395ed" />


Before the CAD modeling I had to sketch what it might look like. I decided to just do a simple box that was capped. I gave the inside a little bit of room in case of expansion during heating. At first I went with a snap fit but found it to be too complicated so instead I have 1/16 inch holes on each corner for a nut and bolt connection.

### CAD Modeling

#### The Bottom
<img width="1124" height="717" alt="1" src="https://github.com/user-attachments/assets/293919ce-f69a-4de1-8721-73fd745fd667" />
<img width="1053" height="669" alt="2" src="https://github.com/user-attachments/assets/b2b71e94-cdab-4f86-8727-647f76de1f92" />
<img width="1160" height="674" alt="3" src="https://github.com/user-attachments/assets/4c6bb6fe-5645-4b2a-bcb2-c816a8fd0ff2" />
<img width="1144" height="713" alt="4" src="https://github.com/user-attachments/assets/54ecbbd0-7922-449d-ba15-4a3d1395d617" />


Modeling in Solidworks was fairly simple. First I made the bottom of the box. This was just a cube that was shelled then added flanges on the box. I made it .2 inches deep in order to provide room for the gears. I then added a hole for the bigger shaft to slide through and the holes on the corner.

#### The Top

<img width="1075" height="679" alt="5" src="https://github.com/user-attachments/assets/d7ac613f-b374-406a-a86c-587655d1f64b" />


I then made the top which was essentially the same thing. This time the hole was on the other side and smaller. I had to make sure the 1/16 inch holes were in the same exact position that way they would line up in assembly.

#### Shafts and Gears
<img width="268" height="450" alt="7" src="https://github.com/user-attachments/assets/d1029506-7fc1-4642-875a-b3f78bde9ce3" />
<img width="289" height="426" alt="6" src="https://github.com/user-attachments/assets/65f198d9-3d37-4200-8084-ba8e5c4e66ae" />
<img width="313" height="358" alt="8" src="https://github.com/user-attachments/assets/3401708f-3572-46ce-a9e8-bd2aac5d0c0d" />
<img width="464" height="461" alt="9" src="https://github.com/user-attachments/assets/291632be-c1f5-408f-841c-c5ce2055e1d0" />

The shafts were just cylinders and the gears were downloaded from McMaster.com.

#### Assembly

Finally I just had to assemble the box. This again was simple. I added each component and mated them all together. Admittedly, I couldn't find a good way to mate gears so they just sit there and are offset from the bottom of the box. Either way I was happy with the final result.

<img width="832" height="563" alt="Last" src="https://github.com/user-attachments/assets/7386c0ff-e4de-444e-91b9-f4bbfd869d90" />


## Decide
In this assignment I had to decide a lot. One of the biggest decisions was how to make the box. I think my design was simple and clean. I enjoyed making it and was proud of the design.

## Communicate
In this assignment I learned how to find a material based off of the pressure and velocity. This is very helpful for multiple situations and is a good tool to have in my belt.

### CAD Files
