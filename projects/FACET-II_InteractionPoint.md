---
layout: project
title:  "FACET-II Interaction Point"
---

## Project Overview

{:style="text-align: center;"}
![FACET-II IP Top View](/assets/img/FACETII-IP_TopView.jpg){: width="960"}

* __Challenge:__ Design and build an experimental apparatus that allows switching between and operating seven experiments remotely.
* __Solution:__ I implemented and executed a requirements-based design process with detailed planning prior to building and commissioning.
  * Developed the layout and design using top-down modeling in SolidWorks.
  * Collaborated with experiment owners to refine requirements and ensure the final design met their needs.
  * Created detailed SolidWorks models for clearance checks and comprehensive BOMs.
* __Result:__ The apparatus successfully supported multiple experimental campaigns, leading to high-impact results.
  * Total system design, construction, and commissioning took just over one year.
  * The system has proven to be highly reliable.

## FACET-II Facility

The FACET-II (Facility for Advanced Experimental Tests) particle accelerator accelerates 2 nC electron beams up to 10 GeV using approximately 1 km of the radio-frequency cavities from the middle third of the original SLAC linac. The facility is unique in its ability to produce very-high-current electron beams, exceeding 100 kA, at 10 GeV. These beams enable a broad range of scientific studies, including plasma wakefield acceleration, strong-field quantum electrodynamics, strong-field physics, and advanced beam diagnostics.

A broad experimental program requires different setups at the accelerator's interaction point (IP). However, access to the IP is limited to two days every two weeks due to radiation from the upstream accelerator. Further complicating setup changes, the IP is located 100 meters from the nearest staircase—spanning three stories—in a tunnel where temperatures regularly exceed 95°F. In this challenging environment, the experimental setup must be highly reliable, support multiple experiments simultaneously, allow for remote switching between configurations, and remain adaptable to future experimental needs.

## Experimental Area

{:style="text-align: center;"}
![Ip area](/assets/img/IPArea.jpg){: width="760"}

The experimental area encompasses the region after the final magnets, where the accelerated beam is brought to a focus. In addition to the electron beam, laser pulses from a 10 TW ultrafast Ti:Sapphire laser system are available. Depending on the experiment, the electron beam interacts with a solid, gas, or plasma target, or directly with the laser. In some cases, the plasma target is ionized by the laser; in others, by the beam. Some experiments focus solely on changes to the electron beam, while others require ultrafast optical diagnostics of the interaction.

The challenge was to design an apparatus that could accommodate these many different modes of operation, enable remote alignment, and switch configurations without requiring physical access.

I developed the design for the experimental apparatus, working extensively with multiple experimental collaborations to ensure it met all requirements.

__The design work involved:__

* Overall layout of the setup and motion strategy.
* Optical design of laser and experimental diagnostics.
* Opto-mechanical design of optical mounts and adjustments.
* Mechanical design of brackets, support structures, and vacuum hardware.
* Cabling layout for the extensive motorization.

__I then developed a schedule, procured the hardware, assembled, and commissioned the setup.__

### Picnic Basket Chamber

The "Picnic Basket Chamber," named for its lid-opening mechanism, is the primary experimental chamber at the IP. Originally used in FACET, the chamber was repurposed for FACET-II with entirely new internal components and updated flanges, which I designed.

{:refdef:style="text-align: center;"}
![Picnic Basket CAD](/assets/img/PicnicBasketCAD.jpg){: height="280" style="margin: 0 6px;border-radius: 5px"}
![Picnic Basket interior](/assets/img/PicnicBasketInterior.jpg){: height="280" style="margin: 0 6px;border-radius: 5px"}
{:refdef}

The chamber contains 45 motorized degrees of freedom. These allow the seven major assemblies to be inserted and aligned with the electron beam vector while also providing laser alignment capabilities for probe lasers, laser-ionized plasma sources, and colliding the focused laser with the electron beam.

{:refdef:style="text-align: center;"}
![Picnic Basket port](/assets/img/PicnicBasketPort.jpg){: height="320" style="margin: 0 6px;border-radius: 5px"}
![Picnic Basket drawing](/assets/img/PBDrawing.jpg){: height="300" style="margin: 0 6px;border-radius: 5px"}
{:refdef}

### Compressor Chamber

The pulse compressor for the laser system is located in a dedicated chamber just upstream of the Picnic Basket Chamber. The pulse compression gratings and mounts existed from FACET but their relocation into a new chamber required designing a new optical path and several new assemblies to support experiments.

{:style="text-align: center;"}
![Compressor CAD](/assets/img/CompressorCAD.jpg){: height="350"}

### Upgrades

The setup in the IP needs to evolve with the demands of the experimental program. Several upgrades have been installed over the last three years, the most significant being a dark field shadowgraphy laser line that necessitated significant changes to the target mount assembly. I oversaw the integration process, built the new assembly, and wired the system.

{:refdef:style="text-align: center;"}
![Dark shadow assembly](/assets/img/DarkShadowAssembly.jpg){: width="550" style="margin: 0 6px;vertical-align:middle;border-radius: 5px"}
![Dark shadow installed](/assets/img/DarkShadowInstalled.jpg){: width="350" style="margin: 0 6px;vertical-align:middle;border-radius: 5px"}
{:refdef}

## Other Photos

{:refdef:style="text-align: center;"}
![Picnic Basket CAD](/assets/img/HeNeBeamline.jpg){: height="400" style="margin: 0 6px;border-radius: 5px"}
{:refdef}
