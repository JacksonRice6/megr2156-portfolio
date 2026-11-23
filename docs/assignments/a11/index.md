# A11 – Motor Selection

## Objective  
Our objective this week is develop the motorized drive and structural integration for the 2kN tester, focusing on motor selection, mounting, frame stability, and clamp design. This phase will ensure that the crosshead moves smoothly under controlled torque and speed while maintaining precise load alignment and secure specimen gripping. The motor selection will be based on our data calculated last week through the analysis of the leadscrew, flange, nut, frame and crosshead.  

Key Constraints: 
- No electronics, no software: purely mechanical.
- Load capacity: 2kN (with appropriate safety factor in structure and drivetrain).
- Speed range: 1-50 mm/min (achieved via lead screw selection).
- Form factor: bench-top footprint favored; manageable overall height; 18 inch lead screw minimum
- Safety Factor : 4

Outline:  
1): Motor Selection  
2): Designing Motor Bracket housing  
3): Select or designing coupler  
4): Select connectors for frame
5): FEA for the top of frame  
6): FEA on vertical components of frame  
7): Designing a floating bearing mount  
8): Tabulation  
9): Lessons learned   

## Analyze
### Motor Selection

From the last assignment i learned that with my 1/4 inch lead screw the required toque for each motor would be .6786 N-m and the rotational speed range for this torque is .63 - 31.5 RPM. Based off of this i reachred a;l type of motors and landed on the Nema 23 Bipolar 3Nm(425oz.in) 3.5A 57x57x113mm 4 Wires CNC Stepper Motor. 

<img width="540" height="540" alt="image" src="https://github.com/user-attachments/assets/a9306788-8055-40eb-89f0-86b30ad749fe" />

<img width="950" height="364" alt="image" src="https://github.com/user-attachments/assets/0ac5e6cb-f92c-410a-b298-e465024c991c" />

[Link to Motor](https://www.omc-stepperonline.com/nema-23-bipolar-3nm-425oz-in-3-5a-57x57x114mm-4-wires-cnc-stepper-motor-23hs45-3504s)

The reason i selected this motor is because first it is a steeper motor which allows it to control its speed and also knows its location so it can be used for precise movements. Second it has a 3nm torque rating which is well above the required torque of .6786 N-m so it has a built and safety factor. Also by looking at its torque speed graph we can see that under 31.5 RPM it still has a output torque of 2.67 N-m which is plenty for this lead screw design. 

<img width="2283" height="900" alt="image" src="https://github.com/user-attachments/assets/1c939854-628e-4b80-bd0a-d9fcbe5aabbe" />

### Motor Mount  
In order to design the motor mount I had to find the thickness the material needed to be. First I selected the material to be 1100 aluminum because it was cheap and the yield strength was more than enough for what I needed. Next I designed it with the dimensions of the actual motor in mind. I mad a casing just big enough for the motor to slide into the holes aligned properly so it could be screwed in. I then calculated the thickness based on two things: the deflection and normal stress. The deflection formula I had to look up to find, then I rearranged it to solve for thickness assuming a max deflection of one millimeter. I also calculated the normal stress using the yield strength of my material. Both used a safety factor of 2. The thickness for max deflection was far greater and was 3.8mm so I designed it with a thickness of 4mm.

<img width="512" height="458" alt="image" src="https://github.com/user-attachments/assets/2cf45992-8f35-43e1-8387-5bf707bb4294" />

<img width="385" height="512" alt="image" src="https://github.com/user-attachments/assets/e58c9cf2-18ff-486f-8804-7b8c9e33f5c7" />

<img width="489" height="512" alt="image" src="https://github.com/user-attachments/assets/67782970-9bc6-4675-8cef-db78df2e2fb6" />

<img width="512" height="311" alt="image" src="https://github.com/user-attachments/assets/492de2d0-5342-4d40-9d16-d0f8680d459f" />


### Coupler Design

The nest thing to do was to design a coupler that would connect the lead screw to the motor shaft. I first started out by listing all my knowns. I knew the internal diameter of the coupler must be 10 mm as that is the shaft size of the motor, the material of the coupler will be steel so its yield strength is 250 MPA, and lastly i know the torque applied to the coupler will be .6785 N-m. From these i know i need to solve for the outer diameter/ size of the coupler so it can withstand the torque applied.  

<img width="1668" height="2157" alt="image" src="https://github.com/user-attachments/assets/4d100abf-f2b9-470c-90fd-44517fef30df" />


From my calculations I see that i need an outer diameter of at least 10.13 mm but i decided to round up to 10.5 mm to be easier to actually manufacture and to have a built in extra safety factor. and here is the dsign for the motor  

<img width="1668" height="641" alt="image" src="https://github.com/user-attachments/assets/ea8b65c9-b40a-4535-ac80-a5d8f5904413" />


### Frame Connectors  

<img width="1520" height="651" alt="image" src="https://github.com/user-attachments/assets/53d73ae8-9a98-426c-84fc-5e48294703a3" />

To select the frame connector, I used my McMasterCarr resources to determine the best fit for our T-Slotted Framing. I determined the 1in x 1in. would be enough surface area to help support the 2000N load, weight and twist of the motors onto the frame. With help of the motor mount, this twist should be significantly reduced.  

[Link to Connector](https://www.mcmaster.com/47065T236/?utm_term=mounted+sleeve+bearings&matchtype=e&campaignid=22711799005&adgroupid=180671261479&location=9009981&gad_source=1&gad_campaignid=22711799005&gbraid=0AAAAACLR9bxAAeR6trfCg2NwrnhPP943C&gclid=CjwKCAiA5Y_YBhBbEiwAK5Dl7cv5DuWSrVLJgJ4cEetm9r8teNK4lYjQCNme6oHTpvSKDxixhAoPXBoCp3wQAvD_BwE)  

### Top Frame FEA

I had to verify that the top of the frame would provide enough strength necessary to withstand the loads of the lead screws and the torque applied by the motors. I took just top frame in CAD and then conducted a FEA simulation where both ends are fixed in place and there are 1kN loads on the frame where the lead screw would be. I also ran two simulations one with a fine mesh and one with a coarser mesh and here they are below. 

<img width="2239" height="844" alt="image" src="https://github.com/user-attachments/assets/b300da6c-e8c2-4fa9-96b6-47701d08f9dc" />

<img width="489" height="408" alt="image" src="https://github.com/user-attachments/assets/75401225-429c-4aa6-8736-1c74e228d089" />

<img width="1282" height="603" alt="image" src="https://github.com/user-attachments/assets/511924e5-592f-482f-b365-4a666a4af78a" />

<img width="856" height="523" alt="image" src="https://github.com/user-attachments/assets/60ca6c14-81f5-4747-9dd5-f7ce371c4830" />

<img width="1549" height="561" alt="image" src="https://github.com/user-attachments/assets/ae3077e9-8e30-4f96-90db-f668230e3459" />

<img width="298" height="238" alt="image" src="https://github.com/user-attachments/assets/b47038a6-e976-4c31-8e38-d9bd07ad8cfb" />

<img width="1595" height="594" alt="image" src="https://github.com/user-attachments/assets/818a313e-869a-4b15-9342-b67246e12028" />

<img width="1484" height="533" alt="image" src="https://github.com/user-attachments/assets/c8559951-b360-4f72-a47c-f8b5f203ced7" />

<img width="1486" height="526" alt="image" src="https://github.com/user-attachments/assets/fc1324b2-bd2c-49b4-9e59-b2df40459d9b" />

From these simulations i calculated a convergence check on the two to verify the results. I got a difference of 7% for the saftey factor, .3% for the displacement, and 7% for the stresses and since all are 7% or under they converge and the results are verified.

Optimization: Looking at the FEA I see that the max stress and bending is where the load from the lead screw connects to the frame. Based from this I would put put square piece of material the size of the frame around these holes made of steel which would be much stronger then the aluminum frame and these square pieces would strengthen and limit the bending of the frame. 

[Link to FEA study](Topframestudy.SLDPRT)

### Side Frame FEA

<img width="919" height="576" alt="image" src="https://github.com/user-attachments/assets/eb90d98f-7c81-4e20-9c3c-d8a09c0cdf38" />

For the FEA on the vertical components I did two studies, one with medium mesh and the other with fine mesh. This was showing compression of the beams. The max deflection I got was 0.0028 inches which is great and the max stress was 1.463 ksi which is far below the yield strength of 31 ksi. The factor of safety was 21 which is very high because the yield strength of our material was far beyond the max stress is experienced.

Cad File:
[SideFrameFEA.zip](https://github.com/user-attachments/files/35299169/SideFrameFEA.zip)



### Mounted Bearing w/ RC3 Class fit  
Justification of each size and location dimension on mount: The bearing bracket sits parallel to the frame of the tensile tester. It will screw into the bottom of the frame using a #9 drill. With the bearing mounts being small, this gives us space to put two with enough distance between them on the frame.  

Noting functional tolerances: RC3 fit for the bearing inner diameter allowing for a slip fit for the lead screw.
#8 screws for the mounting holes, because the diameters allow for little clearance between the chamfer the hole and the head of the screw.  

[Link to Mounted Bearing](https://www.mcmaster.com/4575N33/?utm_term=mounted+sleeve+bearings&matchtype=e&campaignid=22711799005&adgroupid=180671261479&location=9009981&gad_source=1&gad_campaignid=22711799005&gbraid=0AAAAACLR9bxAAeR6trfCg2NwrnhPP943C&gclid=CjwKCAiA5Y_YBhBbEiwAK5Dl7cv5DuWSrVLJgJ4cEetm9r8teNK4lYjQCNme6oHTpvSKDxixhAoPXBoCp3wQAvD_BwE)  

### Bill of Materials and Labor Cost  
Hourly cost for team members was $35 / Hour (median entry-level engineering designer pay)  
[Link to Bill of Materials and Labor Cost](https://docs.google.com/spreadsheets/d/15JimiBi4IxkgIMTaRMZI8nueYGNDZvNTg6ABmjvZoxY/edit?usp=sharing)  

<img width="512" height="439" alt="image" src="https://github.com/user-attachments/assets/095c9938-1109-43a9-b3bc-5aed2d1c2f42" />



## Lessons Learned

Justin Adelman: This assignment taught me how to solve for the thickness needed for a coupler based on the torque being applied and the material of the coupler itself. This assignment also helped me to feel more confident and fluent with running FEA's and interpreting the results to help with verification of the loads and optimization for the design.  

Justin Hatcher: One particular lesson I learned during this assignment was how to use AI, McMasterCarr, and torque curve more effectively to search for the information I wanted. This significantly streamlined the process compared to A10, and with the additional research from that previous assignment. I was about to work, quicker, and faster compared to the previous weeks.  
