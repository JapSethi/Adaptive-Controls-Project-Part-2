# <div align="center">Adaptive-Controls-Project-Part-1</div>
**<div align="center"> To design a [model reference adaptive controller](http://www.phoneoximeter.org/uploads/media/EECE574-11_MRAC_01.pdf) for a DC motor drive, which accounts for the presence of an unknown deadzone in the power electronincs, so that the approximate velocity tracking may be achieved without knowledge of motor, load or deadzone parameters.</div>**

> **Note: Part 2 of the Project deals with Model Reference Adaptive Control of Full Output Feedback DC motor drive system**


### Background:
<p align="center"><img src="Brushed DC Motor.JPG"> </p>

 #### Dynamics of the **brush-commutated permanent-magent DC motor** turning an inertial load are described by:


<p align="center"><img src="Background.JPG"> </p>

### Overview (For Part 2):

<p align="center"><img src="Overview_Part2.JPG"> </p>

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
