---
course_id: es-293-lego-robotics-spring-2007
layout: course_section
parent_title: SP.285
title: Control of a Plotter
type: course
uid: 57a2e97039bf2e691831a4194ccc949e

---

[SP.285]({{< baseurl >}}/sections/sp.285)

Chad Keever, [Projectile Launcher]({{< baseurl >}}/sections/sp.285/keever_index)  
Kendall McConnel, Control of a Plotter  
Jonah Elgart, [Guidance by IR Beacon]({{< baseurl >}}/sections/sp.285/index_bologna)  
Miki Havlickova, [IR Remote Control]({{< baseurl >}}/sections/sp.285/index_mikihavl)  
Jessica Bowles-Martinez, [Guidance by Light]({{< baseurl >}}/sections/sp.285/index_jnbm)  
Matt Seegmiller, [Master/Slave IR Control]({{< baseurl >}}/sections/sp.285/index_xaco)  
Jitin Asnaani, [Invertible Robot]({{< baseurl >}}/sections/sp.285/index_jitin)

* * *

![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/8c1052b0903dfd7bf48a68824e2bcaa7_pic3.jpg)

Hello! My name is Kendall McConnel and this webpage is devoted to my final project for [SP.285]({{< baseurl >}}/sections/sp.285), a seminar on Robotics and Mechatronics.

First, a little bit about the class...

The Robotics and Mechatronics seminar is taught in ESG by two spiffy fellows by the names of Eric Smith and Max "Ben" Davis. The course involves tinkering with Legos, motors, sensors and programming to create robots that can pick up, run away from light, or even follow a line. For the first part, I learned about how to make a robot and what goes into making it work. Max and Eric ran lectures on topics related to the robots (sensors, electronics, etc) and also helped us work through and learn about what works best. For the latter part, I worked on a project (this one) which reflects my interest in programming specifically.

And now, a bit about my project!

I chose to work with a plotter (which came with two sensors and two motors) my plan was to get the plotter to go to a point as accurately as possible, and, if time allowed, to draw simple objects.

The main problem of this particular plotter was that because it was so smooth (barely any friction) it would overshoot and wouldn't be very accurate. So, part of my project was to learn a bit about control theory and apply and test different methods to see what worked best.

To sum up my experience with my plotter, I tinkered with different functions of distance to see what would get the plotter to the designated point as quickly and as accurately as possible. First, I wrote up readpt function that would give out the x coordinate on the plane. Then, I tried different gotox functions. Initially, I tried a simple distance function (but when the motor runs too slow, it doesn't move and sounds horrible so.) then I experimented with different sections where the motor would run at different speeds (i.e. at the distance for speed, and then, when it got close enough, (within a certain distance) it would run at a minimum speed.) I still had a decent degree of overshoot and some bugs, but after awhile I created a distance function that worked. To make the geometrical figures that my plotter eventually drew, I created a line function (that makes a diagonal line out of smaller lines) for a complete record of what I did on a day to day basis, check out my journals ([TXT](./resolveuid/e47a347f5a4489c95fea0698038b2045)). And, if you're **really** curious, you can check out my program ([C](./resolveuid/9b8889e8d59f30ffc93cd599e7cbc6de)).

And now, some pictures of my monster (I mean, my... uh.. creation)

![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/88bf8c15458131b55f299ff044a7c2df_pict1.jpg) ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/8914289a8b1067527d895cf25bf83ad1_pic4.jpg) ![Student Lego Project.](/coursemedia/es-293-lego-robotics-spring-2007/779a233fa680578f97f1fea72dbe4c61_pict2.jpg)