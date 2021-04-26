---
course_id: es-293-lego-robotics-spring-2007
layout: course_section
parent_title: SP.285
title: Guidance by IR Beacon
type: course
uid: 71bf2a2a5a80abb96b63accb8c525add

---

[SP.285]({{< baseurl >}}/sections/sp.285)

Chad Keever, [Projectile Launcher]({{< baseurl >}}/sections/sp.285/keever_index)  
Kendall McConnel, [Control of a Plotter]({{< baseurl >}}/sections/sp.285/index_kendallm)  
Jonah Elgart, Guidance by IR Beacon  
Miki Havlickova, [IR Remote Control]({{< baseurl >}}/sections/sp.285/index_mikihavl)  
Jessica Bowles-Martinez, [Guidance by Light]({{< baseurl >}}/sections/sp.285/index_jnbm)  
Matt Seegmiller, [Master/Slave IR Control]({{< baseurl >}}/sections/sp.285/index_xaco)  
Jitin Asnaani, [Invertible Robot]({{< baseurl >}}/sections/sp.285/index_jitin)

* * *

Hi, I'm Jonah Elgart and for my final project in [SP.285]({{< baseurl >}}/sections/sp.285), a robotics and mechatronics class taught in [ESG](http://esg.mit.edu/) (Experimental Study Group), I created a Lego robot that chases or flees an infrared beacon.

My robot car is very simple. It has two wheels, each connected to its own motor. The two motors are driven at different speeds to steer the car. The back wheel is mounted on a really cool caster that I built with Eric (one of the instructor dudes).

|  {{< br >}}{{< br >}} ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/509414d73f51a5492ca71d004033ae32_robot.jpg) {{< br >}}{{< br >}} My robot. {{< br >}}{{< br >}}  |  {{< br >}}{{< br >}} ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/eeb16f9522497425247a4c719c3e8e01_robot_low.jpg) {{< br >}}{{< br >}} The car. {{< br >}}{{< br >}}  |  {{< br >}}{{< br >}} ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/6486d3393749f2451fac559c8233334d_robot_rear.jpg) {{< br >}}{{< br >}} The car's rear side. {{< br >}}{{< br >}}  

|  {{< br >}}{{< br >}} ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/ea38ec08f85f9d7ffe7547077661707c_ir_transmiter.jpg) {{< br >}}{{< br >}} Infrared transmitter. {{< br >}}{{< br >}}  | An infrared signal is broadcasted from a transmitter hooked up to a handyboard (one of those circuity things which is a minicomputer). |
|  {{< br >}}{{< br >}} ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/131a2a83629e8edb0af8719b986fdfac_ir_tower.jpg) {{< br >}}{{< br >}} Infrared receiver. {{< br >}}{{< br >}}  | The signal is detected by the tower, which consists of three directional infrared receiver doohickeys, oriented in three quadrants. 

Click "code" ([C](./resolveuid/a5282be50ae5c190eb88b1d978c7bf9d)) to see the IC code I wrote to make the robot flee or chase the signal. To change from flee to chase you simply reverse the polarity of the motors.