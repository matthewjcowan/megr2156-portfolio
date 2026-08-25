# A1 – Portfolio and Product Analysis

## Objective
To show an understanding of how and why engineering designs work, not just the final result. Evaluate two engineering portfolios based on how well they communicate and organize engineering work, then choosing a simple mechanical product and explaining its function, the mechanical principles behind it, how its geometry affects its performance, and the reasoning behind its design choices.

## Analyze
### Task A: Portfolio Analysis

__Portfolio 1:__ Paul Khoury (Github Pages) https://khourypaul.github.io/portfolio/ 

__Navigability:__ The portfolio uses a central project list containing numerous projects, including CAD, FEA, machine learning, prosthetics, and mechanical design work. A reader can likely locate a named project in under 60 seconds because the projects are listed together on the main page. Because the portfolio is structured by project title instead of by course, analysis type, or assignment, finding a particular technical result often requires opening individual files or pages.

__Reproducibility:__ Reproducibility is different for each project. The portfolio includes technical reports and presentation materials for some projects, such as a detailed haptic system report. These materials give more information about the problem, design goals, testing process, and engineering decisions than the project summaries alone. However, the portfolio does not always include complete CAD files, source data, calculations, dimensions, or detailed instructions. Because of this, another mechanical engineering student could understand how some projects were completed but might need additional information to fully reproduce every project.

__Evidence of Reasoning:__ This portfolio shows evidence of the thinking and reasoning behind the projects, not just the final results. For example, the haptic project explains the engineering problem, design goal, sensory-feedback method, and testing plan. This helps someone with a technical background understand how the problem led to the chosen solution. However, not every project provides the same level of detail. Some projects mainly include short descriptions, images, or the final product.

__Professional Tone:__ The language in this portfolio is appropriate for employers and other engineering professionals because it clearly describes technical responsibilities, engineering methods, and project work. Technical terms such as CAD, finite element modeling, automation, inverse kinematics, and corrective actions are used to explain actual experience instead of just listing skills. The portfolio also organizes projects, experience, skills, and awards into separate sections, making it easier for employers to quickly evaluate the person’s technical background.


__Portfolio 2:__ Joe Alapat (Personal Site) https://joealapat.com/ 

__Navigability:__ The portfolio uses a layout inspired by SolidWorks, with tabs and a sidebar to navigate through experience, projects, 3D models, skills, and contact information. Someone familiar with CAD software can quickly find the main sections, and the projects are organized in a clear visual structure. However, the layout may take more time to understand than a typical engineering website because the navigation is designed to look like CAD software. A first-time employer or reviewer who is not familiar with this style may have a harder time finding specific information or documents at first.

__Reproducibility:__ The portfolio describes technical systems, such as a high-resolution data collection system, a spray-cooling platform, and an intelligent thermocouple monitoring system. These descriptions explain the main purpose of each system and how the major parts work together. However, the portfolio does not include complete drawings, dimensions, calculations, testing procedures, raw data, or source code. Because of this, another engineer could understand the overall design but would need more information to fully reproduce the project.

__Evidence of Reasoning:__ The portfolio shows some of the reasoning behind the projects by explaining why the systems were designed and what engineering problems they were meant to solve. For example, the JACK system explains how it detects when sensors disagree and how its confidence-based algorithm handles unreliable measurements. The spray-cooling project also clearly explains the thermal problem being studied. However, the portfolio focuses more on what the projects can do and their final results than the full decision-making process. It does not always show rejected design options, engineering equations, calculations, or detailed testing and validation results.

__Professional Tone:__ The technical descriptions use engineering-specific language and clearly explain responsibilities, tools, and how the systems work. Topics such as thermal management, instrumentation, embedded controls, data collection, and experimental platforms support the skills listed in the portfolio. Overall, the portfolio is appropriate for showing technical experience to an engineering employer. However, some project descriptions could be stronger by including measurable results and performance data instead of mainly explaining what was built.

### Task B: Product Analysis

__Product:__ Binder Clip

The selected product is a standard spring-steel binder clip with two wire handles. It meets the three-component constraint because the product can be separated into one clip body and two individual wire handles.

__Primary Function:__ The main function of the binder clip is to generate and maintain a normal clamping force that holds multiple sheets of material together by elastically deforming a spring-steel body. The two wire handles provide a mechanical input that temporarily opens the jaws. When the handles are released, the elastic deformation of the clip body produces a restoring force that closes the jaws and maintains constant pressure on the paper.

__Governing Mechanical Model:__ The primary behavior of the binder clip is governed by elastic deformation and Hooke's law. 

A model of this is __F=kδ__ 

Where:

__F__ = restoring force generated by the deformed clip body

__k__ = equivalent stiffness of the spring steel body

__δ__ = elastic displacement caused by opening the jaws

One assumption is that the spring-steel body remains within its elastic deformation range during normal operation. Under this assumption, the material returns approximately to its original shape after the handles are released, making a linear elastic model such as F=kδ useful.

__Component Geometry and Mechanical Function:__

Component 1: Spring Steel Clip Body:
![Spring Steel Clip Body](f70194c0-b4d6-42e6-87d7-4c5337c3ffe7.jfif) 
The clip body is made from one piece of spring steel that is bent into a triangular shape. This shape creates two flexible sides that meet at the front to form the clamping jaws. The triangular design allows the clip to bend and store energy when it is opened. The curved section at the back is the main area that provides the spring action. When the jaws are opened, the steel bends and stores energy. When the force is removed, the steel tries to return to its original shape, which pulls the jaws back together. The front edges of the clip are curled outward to create rounded areas where the wire handles connect. These curled edges allow the handles to pivot smoothly while also keeping them in place.

Component 2: First Wire Handle
The first handle is made from one continuous piece of wire bent into a loop. The ends of the wire fit into the curled edges of the clip, allowing the handle to pivot. The long shape of the handle gives the user more leverage, so a small hand force can create enough force to open the jaws. When the handle is rotated, it pushes against the clip body and causes the spring-steel sides to bend, which opens the jaws.

Component 3: Second Wire Handle
The second handle has a similar wire-loop design as the first handle but is attached to the opposite side of the clip. Together, the two handles create a balanced opening mechanism. When the user squeezes the handles together, they rotate around their pivot points and open the clip. Using two handles spreads the force across both sides of the clip instead of relying on one handle. The handles can also be folded backward after the clip is attached, which makes the clip more compact and allows the papers to lay flatter. The thickness of the wire is also important. A thicker wire is stronger and bends less, while the continuous wire design provides enough strength to transfer the user's force without needing extra parts.

__Patent Research:__

Patent Number and Inventor: 

A relevant early patent for a binder clip is U.S. Patent No. 1,865,453, “Binder Clip,” invented by Louis E. Baltzley. The patent was filed on February 27, 1930, and published on July 5, 1932. The patent identifies the objective of holding paper and other materials with a construction capable of accommodating varying thicknesses while resisting twisting. Source: https://patents.google.com/patent/US1865453A/en 

A patent more closely representing the geometry of a modern three-component binder clip is U.S. Patent No. 7,120,969, “Binder Clip,” invented by David Carls. It describes a triangular clip body with spring-biased side panels and two pivoting wire levers. Source: https://patents.google.com/patent/US20060130288A1/en 

Alternative Solutions:

Alternative 1: Traditional Paper Clip

A regular paper clip serves the same basic purpose of holding multiple sheets together using contact force and friction. However, instead of using a spring-steel body with jaws, it is made from one piece of wire that bends to create the spring force. Because of its simpler design, a paper clip usually provides less consistent clamping force and is not as effective at holding thicker stacks of paper.

Alternative 2: Spring Jawed Paper Clip
A spring-jawed paper clip uses two opposing jaws and a spring mechanism to hold sheets of paper together. It solves the same basic problem as a binder clip but uses a different design with pivoting arms and spring components. For example, U.S. Patent No. 2,230,450 describes a spring-jawed paper clip that uses actuating arms to open the jaws.

Original Design Decision:

One important design decision is using one bent strip of spring steel to create the triangular clip body instead of separate jaws and a spring. This reduces the number of parts and makes the clip easier to manufacture. The body also performs three main functions: Stores spring energy, Supports the clip structure, and Creates the clamping jaws. The curled edges provide pivot points for the wire handles, allowing them to rotate and open the jaws. These features work together to make the clip simple, strong, and functional.

## Decide


## Communicate

