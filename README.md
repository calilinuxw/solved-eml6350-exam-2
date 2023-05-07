Download Link: https://assignmentchef.com/product/solved-eml6350-exam-2
<br>
This is a open book and open notes exam. Copying someone else’s code or solution is considered a violation of the university honesty policy. NOTE: If you need to make any assumptions, list them (e.g., if you need to restrict the domain, assume some trigonometric property, etc.). UPLOAD A SINGLE

PDF OF YOUR SOLUTIONS AND YOUR CODE IN A SINGLE ZIP FILE ONLINE

<ol>

 <li>Consider the following dynamic system of an actuated pendulum attached to an actuated collar on a track, both with first order actuator dynamics</li>

</ol>

<em>u</em>˙<em><sub>ϕ </sub></em>= −<em>a<sub>ϕ</sub>u<sub>ϕ </sub></em>+ <em>µ<sub>ϕ</sub></em>

where <em>x,x,</em>˙ <em>x</em>¨∈R are the position, velocity, and acceleration of the collar on the track, <em>ϕ,ϕ,</em><sup>˙ </sup><em>ϕ</em><sup>¨</sup>∈R are the angle, angular velocity, and angular acceleration of the mass on the end of the pendulum, <em>m<sub>x</sub>,c<sub>x</sub>,a<sub>x </sub></em>∈R<em>&gt;</em><sub>0 </sub>are the unknown constant mass, friction coefficient, and input coefficient for the collar, <em>m<sub>ϕ</sub>,c<sub>ϕ</sub>,l,a<sub>ϕ </sub></em>∈R<em>&gt;</em><sub>0 </sub>are the unknown constant mass, friction coefficient, arm length, and input coefficient for the pendulum, is gravity, <em>u<sub>x </sub></em>∈R is the output force of the actuator on the collar, <em>µ<sub>x </sub></em>∈ R is the controlled input to the actuator on the collar, <em>u<sub>ϕ </sub></em>∈ R is the output torque of the actuator for the pendulum, <em>µ<sub>ϕ </sub></em>∈R is the controlled input to the actuator for the pendulum (i.e., you cannot directly control <em>u<sub>x </sub></em>or <em>u<sub>ϕ</sub></em>). Design backstepping inputs, adaptive updates, <em>µ<sub>x</sub></em>, and <em>µ<sub>ϕ </sub></em>to control the coupled systems and actuator dynamics and prove the system is stable using the designs. There are two goals for this problem, to have the collar track a desired trajectory that oscillates between −<em>x<sub>d </sub></em>and <em>x<sub>d </sub></em>at a frequency of <em>f<sub>x</sub></em><em><sub>d </sub></em>which we model as <em>x<sub>d </sub></em>(<em>t</em>) = <em>x<sub>d </sub></em>sin(2<em>πf<sub>x</sub></em><em><sub>d</sub></em><em>t</em>) implying <em>x</em>˙<em><sub>d </sub></em>(<em>t</em>) = 2<em>πf<sub>x</sub></em><em><sub>d</sub></em><em>x<sub>d </sub></em>cos(2<em>πf<sub>x</sub></em><em><sub>d</sub></em><em>t</em>) and <em>x</em>¨<em><sub>d </sub></em>(<em>t</em>) = −(2<em>πf<sub>x</sub></em><em><sub>d</sub></em>)<sup>2 </sup><em>x<sub>d </sub></em>sin(2<em>πf<sub>x</sub></em><em><sub>d</sub></em><em>t</em>); while simultaneously, the pendulum tracks the desired trajectory that oscillates between −<em>ϕ<sub>d </sub></em>and <em>ϕ<sub>d </sub></em>at a frequency of <em>f<sub>ϕ</sub></em><em><sub>dd</sub></em>which we model as<sup>2 </sup><em><sub>d </sub></em><em>ϕ<sub>d </sub></em>(<em>t</em>) = <em>ϕ<sub>d </sub></em>sin(2<em>πf<sub>ϕ</sub></em><em><sub>d</sub></em><em>t</em>) implying<sup>… </sup><sup>˙ </sup><em>ϕ,</em><sup>¨</sup><em>ϕ</em><sup>˙</sup><em><sub>d</sub></em><sub>…</sub><em>ϕ</em>(<em>t</em>) = 2are all measurable.<em>πf<sub>ϕ</sub></em><em><sub>d</sub></em><em>ϕ<sub>d </sub></em>cos(2<em>πf<sub>ϕ</sub></em><em><sub>d</sub></em><em>t</em>)

and <em>ϕ</em><sup>¨</sup><em><sub>d </sub></em>(<em>t</em>) = −(2<em>πf<sub>ϕ </sub></em>) <em>ϕ<sub>d </sub></em>sin(2<em>πf<sub>ϕ </sub>t</em>). You can assume <em>x,x,</em>˙ <em>x,</em>¨ <em>x ,ϕ,ϕ,</em>

<ul>

 <li>(50 pts) Design the best stable controller based on what has been shown in class and prove thestability of the designed controller using Lyapunov-based methods. Show all your work.</li>

 <li>(50 pts) READ ALL THE INSTRUCTIONS. PLOTS NOT FOLLOWING THE CORRECT FORMAT WILL NOT GET FULL CREDIT. IF SOMETHING IS NOT CLEAR PLEASE ASK.</li>

</ul>

<ol>

 <li>Using your results of Part (1.a), simulate the dynamics for 100 random values of <em>x<sub>d</sub></em>, <em>ϕ<sub>d</sub></em>, <em>f<sub>x</sub></em><em><sub>d</sub></em>, <em>f<sub>ϕ</sub></em><em><sub>d</sub></em>, <em>x</em>(<em>t </em>= 0), <em>ϕ</em>(<em>t </em>= 0), within your domain but keep</li>

</ol>

<table width="100">

 <tbody>

  <tr>

   <td width="70"><em>x</em>˙ (<em>t </em>= 0)</td>

   <td width="24">=</td>

   <td width="7">0</td>

  </tr>

  <tr>

   <td width="70"><em>u<sub>x </sub></em>(<em>t </em>= 0)</td>

   <td width="24">=</td>

   <td width="7">0</td>

  </tr>

  <tr>

   <td width="70"><em>ϕ</em><sup>˙ </sup>(<em>t </em>= 0)</td>

   <td width="24">=</td>

   <td width="7">0</td>

  </tr>

  <tr>

   <td width="70"><em>u<sub>ϕ </sub></em>(<em>t </em>= 0)</td>

   <td width="24">=</td>

   <td width="7">0</td>

  </tr>

 </tbody>

</table>

and random values for <em>m<sub>x</sub>,m<sub>ϕ</sub>,c<sub>x</sub>,c<sub>ϕ</sub>,l,a<sub>x</sub>,a<sub>ϕ </sub></em>that satisfy your determined conditions (if any). ii. Discuss any algorithms you used for designing your controller.

iii. Plot the results of your Monte Carlo making sure the behavior of the system is clear (i.e., choose a small enough time step, large enough initial conditions, and run the simulation long enough to see the behavior of the system). Specifically,

<ol>

 <li>plot the norm of your tracking errors over time on a single plot</li>

 <li>plot the norm of your estimation errors over time on a single plotiv. Select a single run that represents the typical performance of your design and</li>

</ol>

1

<ol>

 <li>plot the total input, the error feedback portions of the input, and the estimated feedfor-ward portions of the input over time</li>

 <li>plot the value of your Lyapunov function over time along with the best determined the-oretical bound of your Lyapunov function over time</li>

 <li>For each run, calculate the norm of the difference between the total input and the errorfeedback portions of the input over time. Average across all of your runs and plot the resulting average over time (this should show a single trajectory over time)</li>

 <li>For each run, calculate the norm of the difference between the total input and the estimatedfeedforward portions of the input over time. Average across all of your runs and plot the resulting average over time (this should show a single trajectory over time)</li>

</ol>

<ul>

 <li>Based on the plots, use quantitative and qualitative descriptions of the plots and data tosupport you discussion of the following

  <ol>

   <li>Discuss whether your simulation matches your stability result</li>

   <li>Discuss if your controller transitioned from predominantly using error feedback terms tousing the estimated feedforward dynamics over time</li>

   <li>Discuss the bound of your Lyapunov function over time</li>

  </ol></li>

</ul>

2