---
layout: project
title:  "Experimental Control System"
---

## Project Overview

* __Challenge:__ Plasma wakefield experiments using laser-ionized plasmas require precise alignment, which must be completed within a single beamtime shift before accelerator drift sets in.
* __Solution:__ I developed control panels, automated tools, and procedures to speed up laser alignment, and feedback systems to help maintain it.
  * Designed task-based GUIs that centralize relevant controls, reducing the number of menus and clicks needed for adjustments.
  * Automated repetitive tasks like aligning a laser to a reference position on a camera or calibrating motors.
  * Developed alignment tools that automate complex multi-step procedures with minimal intervention.
  * Created real-time data analysis displays to provide immediate feedback on experimental results.
* __Result:__ Experimental setup time was reduced to a level where it was possible to complete within a single shift.
  * Reduced laser warmup and alignment time from 2.5 hours to less than 1 hour.
  * Setup time for laser-ionized plasma wakefield accelerator experiments has been reduced from ~8 hours to ~3 hours.

## Laser Control Panels

Controls for the laser system components were spread across a wide number of panels, with some controls placed several menus deep. Finding the menus required knowing things like the controller and rack a motor was connected to. The controls themselves were generic, providing a clunky interface that required significant user input. Take for example changing the laser energy. A user would have to look up that the motor for the waveplate was on controller LS24, click through the following list of menus *FACETHOME->LI20->Laser->Infrastructure->XPS moc-la20-ls24*, look up a plot of energy vs. angle in the laser wiki to figure out what angle to use, then enter the angle desired into the "Request" box. Performing such a long process 10s of times during laser alignment significantly increased the time required.

I designed new laser control panels, organizing them into three logical sections, each with a dedicated interface containing all relevant controls. This allows alignment to proceed by working through the panels one after another. The final panel contains all the controls required for running the experiment in one place. Each control includes device-specific buttons based on what I felt was most useful for the user. Instead of a generic motor control, for example, the energy attenuator waveplate has buttons in terms of energy percentage.

{:refdef:style="text-align: center;"}
![Laser room control panel](/assets/img/LaserRoomControlPanel.jpg){: width="960" style="border-radius: 5px"}
![Tunnel control panel](/assets/img/TunnelControlPanel.jpg){: width="700" style="border-radius: 5px"}
{:refdef}

The best feature of the laser control panels is the "Auto" button on each alignment camera. Click it once and the associated steering mirror aligns the laser to the reference position.

## Experiment Automation and Live Data Analysis

{:refdef:style="text-align: center;"}
![Chernekov spectrometer](/assets/img/CHERWaterfall.jpg){: width="960" style="border-radius: 5px"}

Real-time access to experimental results is essential for rapid tuning and optimization. I wrote a spectrometer analysis tool that extracts the electron beam energy spectrum from the raw Cherenkov spectrometer images in real time, eliminating the need for post processing. The tool calculates several parameters from the spectrum that have been used as objective functions for machine-learning-based accelerator optimization. It also provides a live waterfall plot of the spectrum which is invaluable for hand tuning the accelerator.

{:refdef:style="text-align: center;"}
![Lithium oven panel](/assets/img/LithiumOvenDisplay.jpg){: height="360" style="margin: 0 6px;border-radius: 5px"}
![EOS panel](/assets/img/EOSPanel.jpg){: height="360" style="margin: 0 6px;border-radius: 5px"}
{:refdef}

Automating tedious, repetitive tasks was crucial to significantly reducing setup time for complex experiments, allowing for more efficient use of beamtime. One of the plasma sources used at FACET-II is a lithium vapor oven that requires 8 hours to reach its operating temperature of 850°C. I wrote automated startup and shutdown scripts to ramp the heater power and monitor the oven temperature during the long heating/cooling cycles. I also wrote a tool for the electro-optic beam measurement system that automatically scans for the signal.

The most sophisticated tool I built is for aligning the laser to the electron beam, the most time-consuming part of using a laser-ionized plasma source. The alignment process relies on scanning the laser-ionized plasma across the electron beam and looking at the light emission on two cameras at different longitudinal positions. The lens system and final steering mirror are then adjusted to bring the laser and electron beam into alignment. The process is extremely tedious to do by hand, and the automated tool reduced what was a 2–3-hour task to less than 20 minutes.

<!-- ## Feedbacks to Stabilize Drift

The laser transport from the laser room to the tunnel passes throught the surface building located above the accelerator housing. This building has no temperature regulation, resulting in part of the laser transport undergoing the full outside day-night temperature cycle. The result is a significant alignment drift throughout the day. This is stabilized using a feedback  -->
