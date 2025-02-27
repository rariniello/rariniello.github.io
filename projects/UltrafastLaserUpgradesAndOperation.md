---
layout: project
title:  "Ultrafast Laser Upgrades and Operation"
---

## Project Overview

{:refdef:style="text-align: center;"}
![Pointing jitter](/assets/img/PointingJitter.jpg){: height="220"}
![Wavefront](/assets/img/S20Wavefront.jpg){: height="220"}
![SSA measurement](/assets/img/SSAMeasurement.jpg){: height="220" style="border-radius: 5px"}
{:refdef}

* __Challenge:__ The FACET-II experimental laser was initially unable to ionize a long H₂ plasma with an axicon lens, despite having sufficient energy.
* __Solution:__ I installed diagnostics to fully characterize the pulse and systematically identified and corrected performance-limiting factors.
  * Built a setup to quickly measure the pulse duration using a single-shot autocorrelator.
  * Modified the adaptive optics setup to enable wavefront measurements closer to the final optics.
  * Created procedures to measure spatial chirp, spectrum, collimation, beam size/profile, and pointing stability.
  * Developed a technique to measure wavefront quality in situ, optic by optic.
  * Implemented periodic characterization to catch and correct performance degradation early.
  * Standardized measurement documentation to ensure long-term consistency.
* __Result:__ Laser intensity on-target increased fivefold, and the laser delivered its specified parameters on 97% of experimental shifts.
  * Discovered and mitigated an issue with the compressor gratings rotating during vacuum pump-down.
  * Identified and replaced out-of-spec optics.
  * Achieved reliable H₂ ionization with an axicon lens after improvements.
  * Enabled high-impact strong-field quantum electrodynamics experiments by increasing a₀.

## FACET-II Laser System

The FACET-II experimental area features an 800 nm Ti:Sapphire laser system producing 600 mJ pulses at the exit of the main amplifier. After amplification, the pulse is image-relayed to a series of diagnostics, a variable energy attenuator, a beam-expanding telescope, and a deformable mirror before being transported through a 30-meter-long vacuum transport line to the accelerator housing. In the accelerator housing, the laser is split into a probe arm and a main arm, each compressed separately to a 45 fs pulse duration. The main arm delivers 225 mJ to the target.

{:style="text-align: center;"}
![S20 laser assembly](/assets/img/Sector20LaserAssembly.jpg){: width="650"}

## Adaptive Optics and Auto Alignment

The laser system was originally built for FACET. For FACET-II, the transport line was rebuilt to reduce the number of windows in the transport line down to a single vacuum entrance window. As part of this redesign, all of the optics after the amplifiers were removed to make way for the new parts of the transport.

I was responsible for designing, installing, and commissioning the new post-amplifier section, which included an attenuator, beam expander, deformable mirror, and alignment diagnostics. I completed this work in parallel with designing the interaction point region.

{:refdef:style="text-align: center;"}
![S20 laser pre-install](/assets/img/S20LaserPreInstall.jpg){: width="460" style="margin: 0 6px;border-radius: 5px"}
![S20 laser room](/assets/img/S20LaserRoom.jpg){: width="460" style="margin: 0 6px;border-radius: 5px"}
{:refdef}

## Laser Diagnostics

Operating a laser system in the high-radiation environment of the accelerator housing presents unique challenges. Complex electronic devices, such as cameras, fail over time due to radiation damage. This makes permanent installations of expensive components—such as deformable mirrors, wavefront sensors, or a single-shot autocorrelator—cost-prohibitive. To avoid destroying expensive components, diagnosing the laser at the interaction point (IP) area originally required setting up and immediately tearing down diagnostic equipment to perform a single measurement, a time-consuming process. Consequently, the laser was primarily characterized in the laser room, and only infrequent checks were performed at the IP. As a result, aberrations introduced during transport often went undetected.

I addressed this issue by building dedicated diagnostic setups in the accelerator housing with kinematic mounts for sensitive detectors. These mounts enabled rapid installation and removal of diagnostic equipment with minimal realignment. Where precise alignment was required—such as for the single-shot autocorrelator—I implemented visible diode laser alignment aids to streamline the process. Finally, I established a regular diagnostic cadence to identify and correct issues before they impacted the science program.

{:refdef:style="text-align: center;"}
![Wavefront setup](/assets/img/CompressorNearFarBuild.jpg){: height="400" style="margin: 0 6px;border-radius: 5px"}
![Visible alignment](/assets/img/CompressorNearFarVisAlignment.jpg){: height="400" style="margin: 0 6px;border-radius: 5px"}
![SSA telescope](/assets/img/DSHMNearFar.jpg){: height="400" style="margin: 0 6px;border-radius: 5px"}
{:refdef}
