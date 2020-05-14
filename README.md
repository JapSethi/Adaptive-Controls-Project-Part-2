# <div align="center">Adaptive-Controls-Project-Part-1</div>
**<div align="center"> To design a [model reference adaptive controller](http://www.phoneoximeter.org/uploads/media/EECE574-11_MRAC_01.pdf) for a DC motor drive, which accounts for the presence of an unknown deadzone in the power electronincs, so that the approximate velocity tracking may be achieved without knowledge of motor, load or deadzone parameters.</div>**

> **Note: Part 2 of the Project deals with Model Reference Adaptive Control of Full Output Feedback DC motor drive system**


### Background:
<p align="center"><img src="Brushed DC Motor.JPG"> </p>

 #### Dynamics of the **brush-commutated permanent-magent DC motor** turning an inertial load are described by:


<p align="center"><img src="Background.JPG"> </p>

### Overview (For Part 1):

<p align="center"><img src="Overview_Part2.JPG"> </p>

### Tasks List:
**Steps taken to develop a MRAC controller**
- Finding the equations (Reduced 1st order or 2nd order equations [**In canonical form**]) and replace coefficents with constant star elements.
- Specify the **Desired trajectory** and find it's derivative.
- Write the equation of **reference trajectory** & its derivative with reference controller element (r).
- Writing the **Reference Error dynamics (er)** equation and it's derivative, and equate the derivative of er to eventually find the reference controller element (r).
- Chose the **controller** with it's star coefficients (theta_x and theta_r) star elements.
- **Close the loop** of your equations and find **Compatibility equations** by comparing it with the reference trajectory equations and thus eventually finding the star elements of the controller (theta_x and theta_r).
- Write **Error Dynamics (e)** equation and it's derivative, equate the derivative of e along with closing it's loop with our controller u to eventually find the derivative of e in terms of e, r and star values.
- Find an appropriate **Lyapunov Function** and it's derivative.
- Making use of the condition that for **stability** the derivative of the Lyapunov Function needs to be **strictly negative** which will make our Lyapunov Function monotonically decreasing, we equate some terms of that derivative of Lyapunov to help us compute the derivative of adaptive theta_x and theta_r values.

> **Note**: In the above steps if we replace our controller's star coefficients with adaptive coefficients then we have devised MRAC system.



### Results: 
## <div align="center">Full Output Feedback System</div>

<p align="center"><img src="ReducedFirstOrderGraphs.jpg"> </p>


#### Languages Used:
- Matlab
- Simulink

#### Use of each file:
- [**AdaptiveControlsProjectPart2_Sethi.mlx**](AdaptiveControlsProjectPart1_Sethi.mlx) - Executable file with clearly defined problem statement and approach
- [**AdaptiveControlsProjectPart2_Sethi.pdf**](AdaptiveControlsProjectPart1_Sethi.pdf) - Published Document for a quick check of Solutions and Code
- [**AdaptiveControlsProjectPart2_Sethi.slx**](AdaptiveControlsProjectPart1_Sethi.slx) - Simulink Model with clearly defined subsystems of both reduced Order and Full Second Order system
> **Note:** Comment out the portion you are not going to use in both simulink and the .mlx script file.
