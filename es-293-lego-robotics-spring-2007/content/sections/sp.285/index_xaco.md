---
course_id: es-293-lego-robotics-spring-2007
layout: course_section
parent_title: SP.285
title: Master/Slave IR Control
type: course
uid: 59180ea356a18194eb691117c8fae4ea

---

[SP.285]({{< baseurl >}}/sections/sp.285)

Chad Keever, [Projectile Launcher]({{< baseurl >}}/sections/sp.285/keever_index)  
Kendall McConnel, [Control of a Plotter]({{< baseurl >}}/sections/sp.285/index_kendallm)  
Jonah Elgart, [Guidance by IR Beacon]({{< baseurl >}}/sections/sp.285/index_bologna)  
Miki Havlickova, [IR Remote Control]({{< baseurl >}}/sections/sp.285/index_mikihavl)  
Jessica Bowles-Martinez, [Guidance by Light]({{< baseurl >}}/sections/sp.285/index_jnbm)  
Matt Seegmiller, Master/Slave IR Control  
Jitin Asnaani, [Invertible Robot]({{< baseurl >}}/sections/sp.285/index_jitin)

* * *

**Matt's IR Controlled Tank**

|  {{< br >}}{{< br >}} ![side.jpg](/coursemedia/es-293-lego-robotics-spring-2007/21b3b479653d272b6e45bc968e7b8438_side.jpg) {{< br >}}{{< br >}} This is a side view of the tank. {{< br >}}{{< br >}}  | For my final project in [SP.285]({{< baseurl >}}/sections/sp.285), I built an infrared controlled tank out of Legos. The basic idea is that one board acts as a slave and takes commands from another board, which acts as master, through IR signals. These signals are sent in 32 bit bursts along some carrier frequency from the master board to the slave board. |
|  {{< br >}}{{< br >}} ![bottom.jpg](/coursemedia/es-293-lego-robotics-spring-2007/23aa6334f495cc1f3afb482c2892b653_bottom.jpg) {{< br >}}{{< br >}} The differentials of the tank as seen from below. {{< br >}}{{< br >}}  | This tank is driven by two motors, one to control forward and reverse motion and the other to control turning. This is accomplished by connecting two differentials so that on one side, the outputs go in the same direction and on the other they go in opposite directions. This is a little hard to understand, unless you know something about differentials already. To help illustrate what is meant by this, there is a picture of the two differentials on my tank below. |
|  {{< br >}}{{< br >}} ![remote_1.jpg](/coursemedia/es-293-lego-robotics-spring-2007/99b14c3de3e742593eb2e1d92bd12760_remote_1.jpg) {{< br >}}{{< br >}} This is the remote. {{< br >}}{{< br >}}  | The other component of this project is the remote. It is basically an old remote from an RC car that has been taken apart and wired so that its sensors can be plugged into a board. The program that runs on this board checks the values of the sensors corresponding to the forward/backward and side-to-side motors. Based on these values, it sends signals to the board on the tank instructing it as to how fast to drive the motors at.