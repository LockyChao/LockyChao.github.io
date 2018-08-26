---
title: "Trajectory Generation and Control of Quadrotor"
collection: research
permalink: /research/quadrotor
---
This project is related to the trajectory generation and control of a quadrotor. 
For the part of trajectory generation, we implemented B-spline interpolation algorithm with maximum velocity at each point for path tracking.
We also improved another state-to-state algorithm [1] for quadrotor trajectory generation between two points. For the part of control, we designed
multiple controllers for different functions. Fig. 1 shows the whole framework, which is also a combination of trajectory generation and control.
Fig.2 presents the dynamic model of a quadrotor mathematically. Fig.3-Fig.6 are the designed flight controllers for different functions.

 <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_1.png?raw=true" alt="The Whole Framework" 
  style="width: 700px;"/> 
</p>
  <p  align="center">Fig.1 The Whole Framework</p>
 </div>

 <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_2.png?raw=true" alt="Dynamic Model of Quadrotor" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.2 Dynamic Model of Quadrotor</p>
 </div>
 
 
 <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_3.png?raw=true" alt="Geometric tracking controller with Head Direction" 
  style="width: 500px;"/> 
</p>
  <p  align="center">Fig.3 Geometric tracking controller with Head Direction </p>
 </div>

 
 <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_4.png?raw=true" alt="Attitude Controller with Height" 
  style="width: 500px;"/> 
</p>
  <p  align="center">Fig.4 Attitude Controller with Height </p>
 </div>

  <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_5.png?raw=true" alt="Attitude Controller with Thrust" 
  style="width: 500px;"/> 
</p>
  <p  align="center">Fig.5 Attitude Controller with Thrust </p>
 </div>


  <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_6.png?raw=true" alt="Mixed Controller Based on State-to-state Algorithm" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.6 Mixed Controller Based on State-to-state Algorithm </p>
 </div>
 
 A series of experiments are performed on Airsim and Matlab to validate the reliablity and feasibility of the proposed methods. 
 Fig.7-Fig.10 displays the experimental results.

  <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_7.gif?raw=true" alt=" Circumventing Two Columns in a Sinusoidal Trajectory" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.7 Circumventing Two Columns in a Sinusoidal Trajectory</p>
 </div>
 
  <div>
  <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_8.gif?raw=true" alt="Passing Two Circles" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.8 Quadrotor Passing Two Circles</p>
 </div>
 
 
 <div>
 <table>
   <tr>
       <td><img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_9.gif?raw=true"  style="width: 350px;" ></td>
      <td><img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_10.gif?raw=true"  style="width: 350px;" ></td>  
  </tr>
</table>
  <p  align="center">Fig.9 Quadrotor Passing a Window by Tilting</p>
 </div>
 

<div>
 <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_11.gif?raw=true" alt="Fully Actuated Hexarotor" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.10 Fully Actuated Hexarotor </p>
 </div>
 
 Besides, we also performed experiments on a real flight controller system based on an open-sourced flight controller PX4. The control framework is shown in Fig.11. In Fig.12, the quadrotor followed the manipulator automatically through his GPS.
 
 <div>
 <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_12.png?raw=true" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.11 The Control Scheme between PX4 and Raspberry Pi 2B </p>
 </div>
 
  
 <div>
 <p align="center">
  <img src="https://raw.githubusercontent.com/Wenbin-Xu/Wenbin-Xu.github.io/master/images/r1_13.gif?raw=true" 
  style="width: 600px;"/> 
</p>
  <p  align="center">Fig.12 Automatically Following the Manipulator </p>
 </div>
 
## Reference 
[1] Mueller, M. W, M. Hehn, and R. D'Andrea. "A computationally efficient algorithm for state-to-state quadrocopter trajectory generation and feasibility verification." Ieee/rsj International Conference on Intelligent Robots and Systems IEEE, 2013:3480-3486.
