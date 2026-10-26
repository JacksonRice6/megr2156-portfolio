# A7 – [Topic]

## Objective

For this assignment I had to perform a Finite Element Analysis(FEA) on the bracket I designed. I had to run the analysis three times to start each with a different coarseness of a mesh. Once it converged or three attempts had been tried I moved to the outer loop which was modifying the geometry of the bracket to minimize stress, displacement, weight and maximize the factor of safety. I did this until the values were optimized.

## Analyze

### Design I

<img width="1077" height="762" alt="image" src="https://github.com/user-attachments/assets/669fe3b4-492b-4233-b923-7b46ff1f14d5" />

For the first inner loop I did two tests. The first test was with coarse mesh and the second was medium. I needed them to converge within 7% of each other. While the deflection converged, the stress and factor of safety did not. This meant I had to do a third test with a fine mesh. Once the third test was done I made the geometric changes.

### Design II

<img width="970" height="777" alt="image" src="https://github.com/user-attachments/assets/a9e18222-427f-43bd-8cfe-cd7ca6d553b1" />

I made everything 1/3 of the thickness in order to see what would break and see my weak points. I knew that this would fail, but it would help me redesign the model to optimize it. Once again I did the inner loop so I did two tests and they converged this time. This meant I could move onto the next design.

### Design III

<img width="990" height="766" alt="image" src="https://github.com/user-attachments/assets/336b8fcc-4c85-474d-b0d8-134ca00f4d35" />

The last design had a max stress of over one million psi. Obviously this was way outside the boundaries since the yield strength was only around 120000. I saw that all the stress was focused on the part that held the cylinder. To diminish this I added a second one on the other side the it would be distributed through the bracket. This went a lot better. The deflection was a minimum and the max stress was about 30ksi under the yield strength. I would have stopped there but the safety factor was only 1.3 and I wanted it a little more. I only had to do 2 tests because it converged within those two tests.

### Design IV

<img width="1297" height="751" alt="image" src="https://github.com/user-attachments/assets/e54d7f1d-bf5c-4c2d-92fc-a8ccafefcf23" />

For the final design I looked at where the stress and deflection was. It was the bottom plane of the bracket, the cylinder, and the two supports. All I did was slightly increase the thickness of each part. This helped optimize the values while keeping the weight below half a pound which was my goal.


## Decide

For this I had to, reasonably, decide my own boundaries for the values; where I wanted the line to be. I was happy with them and that they were actaully achievable. It gave me a very good, clean result.

## Communicate

In this assignment I learned how to preform an FEA and how useful they can be. You can test a design before spending the money and time to make it. It is a very useful tool that I will be using in the future.

### CAD Files

[Bracket.zip](https://github.com/user-attachments/files/33974576/Bracket.zip)
