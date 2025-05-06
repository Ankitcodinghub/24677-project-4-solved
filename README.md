# 24677-project-4-solved
**TO GET THIS SOLUTION VISIT:** [24677 Project 4 Solved](https://www.ankitcodinghub.com/product/24677-project-4-solved-2/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;96317&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;24677 Project 4 Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
1 Introduction

In this project, you will complete the following goals:

1. Design a EKF SLAM to estimate the position and heading of the vehicle.

[Remember to submit the write-up, plots, and codes on Gradescope.]

</div>
</div>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
2 P4: Problems

Exercise 1. In this final part of the project, you will design and implement an Extended Kalman Filter Simultaneous Localization and Mapping (EKF SLAM). In previous parts, we assume that all state measurements are available. However, it is not always true in the real world. Localization information from GPS could be missing or inaccurate in the tunnel, or closed to tall infrastructures. In this case, we do not have direct access to the global position X, Y and heading ψ and have to estimates them from x ̇, y ̇, ψ ̇ on the vehicle frame and range and bearing measurements of map features.

</div>
</div>
<div class="layoutArea">
<div class="column">
Consider the discrete-time dynamics of the system:

Xt+1 =Xt +δtX ̇t +ωtx Yt+1 = Yt + δtY ̇t + ωty ψt+1 = ψt + δtψ ̇t + ωtψ

SubstituteX ̇t =x ̇tcosψt −y ̇tsinψt andY ̇t =x ̇tsinψt +y ̇tcosψt into(1), Xt+1 =Xt+δt(x ̇tcosψt−y ̇tsinψt)+ωtx

Yt+1 =Yt+δt(x ̇tsinψt+y ̇tcosψt)+ωty ψt+1 = ψt + δtψ ̇t + ωtψ

δt is the discrete time step. The input ut is [x ̇t y ̇t ψ ̇t]T . Let pt = [Xt

</div>
<div class="column">
(1)

(2)

Yt]T . Suppose

</div>
</div>
<div class="layoutArea">
<div class="column">
you have n map features at global position mj = [mjx mjy]T for j = 1,…,n. The ground

truth of these map feature positions are static but unknown, meaning they will not move

but we do not know where they are exactly. However, the vehicle has both range and

bearing measurements relative to these features. The range measurement is defined as the

distance to each feature with the measurement equations yj = ∥mj − pt∥+vj for

</div>
</div>
<div class="layoutArea">
<div class="column">
j = 1, …, n. The bearing measure is defined as the angle between the vehicle’s heading (yaw angle) and ray from the vehicle to the feature with the measurement equations yj =

</div>
</div>
<div class="layoutArea">
<div class="column">
atan2(mj −Y ,mj −X )−ψ +vj

y t x t t t,bearing

the measurement noises. Let the state vector be

</div>
<div class="column">
for j = 1,…,n, where the vj t,distance

 Xt   Yt 

 ψt 

 m1  x  m1  y

</div>
<div class="column">
t,bearing

and vj are t,bearing

(3)

</div>
</div>
<div class="layoutArea">
<div class="column">
xt=m2  x  m2   .y 

</div>
</div>
<div class="layoutArea">
<div class="column">
 .   m nx  mny

</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
<div class="layoutArea">
<div class="column">
t,distance t,distance

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
The measurement system be



 

yt= 



</div>
<div class="column">
∥m1−p∥

</div>
<div class="column">
 v1  t,distance

</div>
</div>
<div class="layoutArea">
<div class="column">
t

</div>
</div>
<div class="layoutArea">
<div class="column">
.

. . 

nn

∥m − pt∥   vt,distance 

</div>
</div>
<div class="layoutArea">
<div class="column">
.

</div>
</div>
<div class="layoutArea">
<div class="column">
1 1 +1  (4) atan2(my −Yt,mx −Xt)−ψt   vt,bearing 

</div>
</div>
<div class="layoutArea">
<div class="column">
..

.   . 

atan2(mn −Y ,mn −X )−ψ vn ytxtt t,bearing

</div>
</div>
<div class="layoutArea">
<div class="column">
Derive Ft and Ht for EKF SLAM to estimate the vehicles state X, Y , ψ and feature positions mj = [mjx mjy ]T simultaneously.

Hints:

• write out the complete dynamical system with the state in (3) and then follow the standard procedure of deriving EKF. Think what is the dynamic for static landmarks?

</div>
</div>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
Exercise 2. For this exercise, you will implement EKF SLAM in the ekf slam.py file by completing four functions (marked with TODO in the script). You can use the same con- troller from your previous parts or write a new one. Before integrating this module with Webots, you can run the script by $ python ekf slam.py to test your implementation. Feel free to write your own unit-testing scripts. You should not use any existing Python package that implements EKF. [Hints: remember to wrap heading angles to [−π, π]]

Check the performance of your controller by running the Webots simulation. You can press the play button in the top menu to start the simulation in real-time, the fast-forward button to run the simulation as quickly as possible, and the triple fast-forward to run the simulation without rendering (any of these options is acceptable, and the faster options may be better for quick tests). If you complete the track, the scripts will generate a performance plot via matplotlib. This plot contains a visualization of the car’s trajectory, and also shows the variation of states with respect to time.

Submit your controller ekf slam.py, ekf slam.py, and the final completion plot as de- scribed on the title page. You do not need to submit the plot generated by running the test script (by running $ python ekf slam.py). Your controller is required to achieve the following performance criteria to receive full points:

1. Time to complete the loop = 250 s

2. Maximum deviation from the reference trajectory = 10.0 m 3. Average deviation from the reference trajectory = 5 m

Debugging tips:

<ul>
<li>Do not hardcode the number of map features. Instead, use n in your code.</li>
<li>Check all the signs carefully.</li>
<li>Check all the numpy array indexing.</li>
<li>Use wrap to pi function smartly. Only wrap the angle terms but not the distance terms.</li>
<li>When you run $ python ekf slam.py, it is normal if the estimation diverge gradually, but you should have some reasonable tracking performance.</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
3 Appendix (Already covered in P1)

</div>
</div>
<div class="layoutArea">
<div class="column">
where ay = dt2

</div>
<div class="column">
inertial

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 1: Bicycle model[2]

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 2: Tire slip-angle[2]

</div>
</div>
<div class="layoutArea">
<div class="column">
We will make use of a bicycle model for the vehicle, which is a popular model in the study of vehicle dynamics. Shown in Figure 1, the car is modeled as a two-wheel vehicle with two degrees of freedom, described separately in longitudinal and lateral dynamics. The model parameters are defined in Table 2.

3.1 Lateral dynamics

Ignoring road bank angle and applying Newton’s second law of motion along the y-axis: may =Fyf cosδf +Fyr

􏰀d2y􏰁

is the inertial acceleration of the vehicle at the center of geometry in the direction of the y axis, Fyf and Fyr are the lateral tire forces of the front and rear

</div>
</div>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
wheels, respectively, and δf is the front wheel angle, which will be denoted as δ later. Two terms contribute to ay: the acceleration y ̈, which is due to motion along the y-axis, and the centripetal acceleration. Hence:

a y = y ̈ + ψ ̇ x ̇

Combining the two equations, the equation for the lateral translational motion of the vehicle

is obtained as:

y ̈=−ψ ̇x ̇+m1(Fyf cosδ+Fyr)

Moment balance about the axis yields the equation for the yaw dynamics as

ψ ̈Iz =lfFyf −lrFyr

The next step is to model the lateral tire forces Fyf and Fyr. Experimental results show that the lateral tire force of a tire is proportional to the “slip-angle” for small slip-angles when vehicle’s speed is large enough – i.e. when x ̇ ≥ 0.5 m/s. The slip angle of a tire is defined as the angle between the orientation of the tire and the orientation of the velocity vector of the vehicle. The slip angle of the front and rear wheel is

αf =δ−θVf αr =−θVr

where θV p is the angle between the velocity vector and the longitudinal axis of the vehicle, for p ∈ {f, r}. A linear approximation of the tire forces are given by

􏰄 y ̇ + l f ψ ̇ 􏰅 Fyf=2Cα δ− x ̇

􏰄 y ̇−lrψ ̇􏰅 Fyr=2Cα − x ̇

where Cα is called the cornering stiffness of the tires. If x ̇ &lt; 0.5 m/s, we just set Fyf and Fyr both to zeros.

3.2 Longitudinal dynamics

Similarly, a force balance along the vehicle longitudinal axis yields:

x ̈ = ψ ̇ y ̇ + a x max = F − Ff

Ff =fmg

where F is the total tire force along the x-axis, and Ff is the force due to rolling resistance

at the tires, and f is the friction coefficient.

</div>
</div>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
3.3 Global coordinates

In the global frame we have:

3.4 System equation

</div>
<div class="column">
X ̇ =x ̇cosψ−y ̇sinψ Y ̇ =x ̇sinψ+y ̇cosψ

</div>
</div>
<div class="layoutArea">
<div class="column">
Gathering all of the equations, if x ̇ ≥ 0.5 m/s, we have:

</div>
</div>
<div class="layoutArea">
<div class="column">
2 C 􏰄 y ̇ + l ψ ̇ 􏰅 y ̈=−ψ ̇x ̇+α(cosδδ− f − r)

</div>
</div>
<div class="layoutArea">
<div class="column">
y ̇ − l ψ ̇ m x ̇ x ̇

</div>
</div>
<div class="layoutArea">
<div class="column">
x ̈ = ψ ̇y ̇ + m1 (F − fmg)

2lC􏰄 y ̇+lψ ̇􏰅2lC􏰄y ̇−lψ ̇􏰅

</div>
</div>
<div class="layoutArea">
<div class="column">
ψ ̈= f α δ− f − r α − r Iz x ̇ Iz x ̇

</div>
</div>
<div class="layoutArea">
<div class="column">
X ̇ =x ̇cosψ−y ̇sinψ Y ̇ =x ̇sinψ+y ̇cosψ

otherwise, since the lateral tire forces are zeros, we only consider the longitudinal model.

</div>
</div>
<div class="layoutArea">
<div class="column">
3.5 Measurements

The observable states are:

3.6 Physical constraints

The system satisfies the constraints that:

</div>
</div>
<div class="layoutArea">
<div class="column">
 x ̇ 

 y ̇ 

  ψ ̇   y = X  Y 

ψ

</div>
</div>
<div class="layoutArea">
<div class="column">
|δ|􏰆π6 rad

F 􏰇0andF 􏰆15736N x ̇ 􏰇 10−5 m/s

</div>
</div>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</div>
<div class="page" title="Page 9">
<div class="layoutArea">
<div class="column">
Name

δ or δf F

m

Cα Iz

Fpq

f delT

</div>
<div class="column">
Table 1: Model parameters. Unit

</div>
</div>
<div class="layoutArea">
<div class="column">
Description

Front wheel angle Total input force Vehicle mass

Cornering stiffness of each tire Yaw intertia

Tire force, p ∈ {x, y},q ∈ {f, r} Rolling resistance coefficient Simulation timestep

</div>
<div class="column">
rad N kg

N

kg mˆ2 N

N/A sec

</div>
<div class="column">
Value

State Input 1888.6

20000

25854

Depends on input force 0.019

0.032

</div>
</div>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
(x ̇, y ̇)

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Vehicle’s velocity along the direction of vehicle frame

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
m/s

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
State

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
(X,Y)

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Vehicle’s coordinates in the world frame

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
m

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
State

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
ψ , ψ ̇

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Body yaw angle, angular speed

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
rad, rad/s

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
State

</div>
</div>
</td>
</tr>
</tbody>
</table>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
lr

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Length from rear tire to the center of mass

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
m

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1.39

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
lf

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Length from front tire to the center of mass

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
m

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
1.55

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
3.7 Simulation

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 3: Simulation code flow

</div>
</div>
<div class="layoutArea">
<div class="column">
Several files are provided to you within the controllers/main folder. The main.py script initializes and instantiates necessary objects, and also contains the controller loop. This loop runs once each simulation timestep. main.py calls your controller.py’s update method

</div>
</div>
<div class="layoutArea">
<div class="column">
9

</div>
</div>
</div>
<div class="page" title="Page 10">
<div class="layoutArea">
<div class="column">
on each loop to get new control commands (the desired steering angle, δ, and longitudinal force, F). The longitudinal force is converted to a throttle input, and then both control commands are set by Webots internal functions. The additional script util.py contains functions to help you design and execute the controller. The full codeflow is pictured in Figure 3.

Please design your controller in the your controller.py file provided for the project part you’re working on. Specifically, you should be writing code in the update method. Please do not attempt to change code in other functions or files, as we will only grade the relevant your controller.py for the programming portion. However, you are free to add to the CustomController class’s init method (which is executed once when the CustomController object is instantiated).

3.8 BaseController Background

The CustomController class within each your controller.py file derives from the Base- Controller class in the base controller.py file. The vehicle itself is equipped with a Webots-generated GPS, gyroscope, and compass that have no noise or error. These sensors are started in the BaseController class, and are used to derive the various states of the vehicle. An explanation on the derivation of each can be found in the table below.

</div>
</div>
<div class="layoutArea">
<div class="column">
Name (X, Y ) (x ̇,y ̇) ψ

ψ ̇

3.9 Trajectory Data

</div>
<div class="column">
Table 2: State Derivation.

Explanation

From GPS readings

From the derivative of GPS readings From the compass readings

From the gyroscope readings

</div>
</div>
<div class="layoutArea">
<div class="column">
The trajectory is given in buggyTrace.csv. It contains the coordinates of the trajectory as (x, y). The satellite map of the track is shown in Figure 4.

</div>
</div>
<div class="layoutArea">
<div class="column">
10

</div>
</div>
</div>
<div class="page" title="Page 11">
<div class="layoutArea">
<div class="column">
4 Reference

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 4: Buggy track[3]

</div>
</div>
<div class="layoutArea">
<div class="column">
<ol>
<li>Rajamani Rajesh. Vehicle Dynamics and Control. Springer Science &amp; Business Media, 2011.</li>
<li>Kong Jason, et al. “Kinematic and dynamic vehicle models for autonomous driving control design.” Intelligent Vehicles Symposium, 2015.</li>
<li>cmubuggy.org, https://cmubuggy.org/reference/File:Course_hill1.png</li>
<li>“PID Controller – Manual Tuning.” Wikipedia, Wikimedia Foundation, August 30th,
2020. https://en.wikipedia.org/wiki/PID_controller#Manual_tuning
</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
11

</div>
</div>
</div>
