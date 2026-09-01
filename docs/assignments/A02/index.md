# A2 – Truss Stress Analysis

## Objective
The objective of this project is to design a lightweight planar truss that supports the two equal and opposite 25 kN loads shown in Figure 1 while satisfying the required geometry, material, and safety-factor constraints. A500 Grade B structural steel is used for the truss members, and hardened tool steel is used for the connecting pins. The design process begins with a statically determinate truss, continues through symbolic and numerical joint analysis, and finishes with a CAD model whose mass properties can be compared with the analytical estimate.
The selected load is P = 25 kN, which lies midway between the allowed 20 and 30 kN values. The specified dimensions are a = 0.4 m and b = 0.3 m. The final geometry uses four joints and five members so that m = 2j - 3 = 5, making the planar truss statically determinate 

## Analyze
### Truss Geometry
The geometry was chosen based on the dimensions given in Figure 1. Points B and A are the upper supports, while points C and D are the lower points where the loads are applied. The three horizontal sections are each a = 0.4 m , and the vertical distance is b = 0.3 m. This design keeps the truss simple by using only five members while still making it statically determinate.
![Truss Geometry](clipuno.jfif) 

#### Member Lengths

### Whole Truss Free Body Diagrams and Reactions

A is modeled as a pin, so it provides Ax and Ay. B is modeled as a roller, so it provides By. Taking moments about A eliminates Ax and Ay and provides the roller reaction. The sign of By is negative, meaning the reaction acts downward for this loading arrangement.

### Method Of Joints

#### Numerical and Symbolic Member Forces

| Member  | Symbolic Force | Numerical Force (kN) | State | Length |
| -------- | -------- | -------- | -------- | -------- |
| BA    |     $\frac{4P}{9}$     |      11.111    | Tension         |       1.2000   |
| BC    |     $\frac{-5P}{9}$     |      -13.889    |   Compression       |     0.500     |
| CD    |  $\frac{4P}{3}$        |     33.333     |    Tension      |   0.400  |
| CA    |  $\frac{-2\sqrt{73}P}{9}$    |    -47.467      |      Compression    |    0.8544      |
| DA    |      $\frac{5P}{3}$    |      41.6667    |   Tension       |      0.500    |

The largest internal force by magnitude is member CA, with Fmax = 47.467 kN. Because every truss member must use the same cross sectional geometry, this member controls the sizing calculation. 

### Member Cross Sectional Area

A500 Grade B structural tubing was selected for the truss members because it has a minimum yield strength of 46 ksi, or about 315 MPa. The design uses this minimum yield strength instead of a higher actual strength to make sure the calculations are based on a conservative value. For each axial member, the allowable stress is found by dividing the yield strength by the required safety factor. 

The theoretical minimum area is 527.4mm2. A practical CAD section of 25mm x 22mm is selected giving A = 550mm2.

The resulting yield-based safety factor is FS = Fy A / Fmax = 3.65, which is greater than the required 3.5

### Approximate Truss Weight

Analytical truss mass, excluding pins: 14.91 kg.

### Pin Design

The pins are designed to be in single shear. To be more conservative, the same pin size is used for the full 25 kN joint load instead of the smaller 8.333 kN support reaction. This approach makes sure the pins can handle the highest load that occurs at any connection in the truss.



A practical pin diameter of 0.500 in was selected for the design. The circular shear area of the pin is 0.1964 in², which results in a shear safety factor of 5.94. This is greater than the required safety factor of 4, so the pin meets the design requirements.

Using a pin length of 22 mm and the given density of the pin material, the four pins have a combined weight of approximately 0.189 lb (0.086 kg).


## Decide
I selected the AB–BC–CD–DA–AC layout, which uses the four-sided frame with one diagonal running from A to C.
The main reason for adding the fifth member was to make the structure stable. The four-member frame alone would act as a four-bar linkage and could deform under the applied loads. With four joints, a planar truss requires five members:
m = 2j - 3 = 2(4) - 3 = 5
I chose AC as the diagonal because it provides the needed bracing without creating a crossing member, making the truss simpler to build. The opposite diagonal would also work, but it would produce a mirror-image design with the same structural behavior.
The given geometry controls the forces and weight of the truss. With a= 0.4 m and b = 0.3 m, the largest internal force occurs in member AC at approximately 47.47 kN in compression. Since the dimensions and material are fixed by the assignment, there was limited opportunity to reduce the weight through geometry. Therefore, the final design focuses on using the minimum practical member size while still meeting the required safety factor.


## Communicate
| Design Item | Final Value |
| :--- | :--- |
| Applied Load | P = 25 kN |
| Geometry | a = 0.4 m, b = 0.3 m; span = 1.2 m |
| Member Section | 25 mm x 22 mm; A = 550 mm^2 |
| Minimum Required Area | 527.4 mm^2 |
| Governing Member | CA; [F] = 47.647kN|
| Member Safety Factor | 3.65 |
|Pin Diameter | 0.500 in |
| Minimum Pin Diameter | 0.410 in|
|Pin Safety Factor | 5.94 |
| Analytical Truss Mass | 14.91 kg |
| Analytical Pin Mass | 0.086 kg |


### Lessons Learned
-Truss geometry must be established before analyzing the forces because the member angles determine the axial-force components at each joint.

-Symbolic equilibrium equations are useful for checking numerical calculations because the load (P) can be kept in the equations until the final substitution.

-When all members have to use the same cross-sectional area, the member with the largest absolute axial force controls the overall member design.

-A safety factor is applied to the material strength to determine the allowable stress instead of directly comparing the applied stress to the material's yield strength.

-A pin in single shear has one effective shear plane, so using the double-shear area would overestimate the pin's capacity.

-CAD mass properties can be used to verify the analytical calculations. Differences between the CAD and hand calculations can be caused by holes, member intersections, geometry, material density, and other modeling assumptions.

### Time
Overall the assignment took me about 11 hours to complete. It was a moderately difficult and labor intensive assignment as we had to create the object in CAD as well. What took the most time was the CAD as it had been a while since I have done CAD work and I needed to refresh myself on how certain things were done within Solidworks.

