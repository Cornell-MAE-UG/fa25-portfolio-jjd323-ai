---
layout: project
order: 1
title: Rocketry Project 2025-2026
description: Year long project focused on insulating and dust-proofing launch-critical ground station. 
technologies: [SolidWorks, 3D Printing]
image: /assets/images/CRT-Logo.png
---


# Fill Station Electronics Enclosure

## Overview

This project focused on the structural and thermal design of an electronics enclosure for a rocket fill station system. The enclosure was designed to:

- Securely mount electrical systems
- Prevent overheating in desert competition environments
- Minimize dust intrusion
- Maintain accessibility for wiring and maintenance

---

# Design Images

## Dust Cover Designs

<div class="image-grid">
  <img src="{{ '/assets/images/DustCover1.png' | relative_url }}">
  <img src="{{ '/assets/images/DustCover2.png' | relative_url }}">
  <img src="{{ '/assets/images/DustCover3.png' | relative_url }}">
</div>

## Board Mount Designs

<div class="image-grid">

  <figure>
    <img src="{{ '/assets/images/DustCover1.png' | relative_url }}">
    <figcaption>Dust Cover 1</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/DustCover2.png' | relative_url }}">
    <figcaption>Dust Cover 2</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/DustCover3.png' | relative_url }}">
    <figcaption>Dust Cover 3</figcaption>
  </figure>

</div>

<div class="image-grid">

  <figure>
    <img src="{{ '/assets/images/PowerBoardMount.png' | relative_url }}">
    <figcaption>Power Board Mount</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/SenseBoardMount.png' | relative_url }}">
    <figcaption>Sense Board Mount</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/SKAM-HatMount.png' | relative_url }}">
    <figcaption>SKAM-Hat Mount</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/SKAMBoardMount.png' | relative_url }}">
    <figcaption>SKAM Board Mount</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/IgnitorBoardMount.png' | relative_url }}">
    <figcaption>Ignitor Board Mount</figcaption>
  </figure>

  <figure>
    <img src="{{ '/assets/images/BallValveBoardMount.png' | relative_url }}">
    <figcaption>Ball Valve Board Mount</figcaption>
  </figure>

</div>

---

# System Function

The system was designed around three primary objectives:

1. Secure mounting of electronic boards
2. Thermal mitigation
3. Dust protection while preserving wire access

Board mounts use heat-set inserts and plastic washers to prevent PCB damage during assembly. Mounts are attached using VHB tape after sanding and cleaning the mounting surfaces with isopropyl alcohol.

Dust covers were designed with wire pass-throughs and sealed using RTV silicone adhesive to reduce dust intrusion while maintaining accessibility.

The enclosure exterior was painted white to reduce solar heat absorption during operation in Midland, Texas.

---

# Requirements

| Requirement | Reasoning | Solution |
|---|---|---|
| Easy board installation | Ease of assembly | Heat-set inserts and screws |
| External port access | Accessibility | Wire pass-through dust covers |
| Secure mounting | Transport safety | VHB + inserts |
| Fit inside enclosure | System integration | CAD-constrained layout |
| Minimize dust entry | Prevent shorts | RTV-sealed openings |
| Thermal mitigation | Prevent overheating | White paint + raised stand |

---

# Thermal Analysis

The dominant heat source for the enclosure was determined to be solar radiation.

The enclosure temperature was modeled using an energy balance derived from the First Law of Thermodynamics:

$$
\alpha G A_{sun}
-
\varepsilon \sigma (T_s^4 - T_{air}^4)
-
h A_{box}(T_s - T_{air})
=
0
$$

| Variable | Meaning |
|---|---|
| $\alpha$ | Solar absorptivity |
| $G$ | Solar irradiance |
| $A_{sun}$ | Projected solar area |
| $\varepsilon$ | Surface emissivity |
| $\sigma$ | Stefan-Boltzmann constant |
| $T_s$ | Surface temperature |
| $T_{air}$ | Ambient temperature |
| $h$ | Convective heat transfer coefficient |
| $A_{box}$ | Surface area |

For glossy white paint:

$$
\alpha \approx 0.1
$$

$$
\varepsilon \approx 0.7
$$

Predicted maximum temperature:

$$
T_{max} = 118^\circ F \approx 47.8^\circ C
$$

This remained below the allowable electronics temperature limit of:

$$
140^\circ F
$$

---

# Manufacturing

Components were manufactured primarily through 3D printing using PETG due to its elevated glass transition temperature.

Manufacturing steps included:

- Sanding mounting locations
- Cleaning surfaces with isopropyl alcohol
- Applying VHB tape
- Installing heat-set inserts
- RTV sealing
- Primer and paint application

---

# Testing

The enclosure system was tested during wet dress rehearsals and hot-fire operations.

Testing feedback resulted in several design iterations, including improved mounting procedures for VHB adhesion reliability.

Thermal validation was analytical rather than experimental due to lack of access to solar simulation facilities.

---

# Bill of Materials

| Item | Supplier | Cost |
|---|---|---|
| VHB Tape | Amazon | \$22.46 |
| White Paint | Home Depot | \$50.94 |
| Heat-set Inserts | McMaster | \$15.22 |
| Plastic Primer | McMaster | \$14.98 |
| Screws | McMaster | \$7.69 |
| Plastic Washers | McMaster | \$12.12 |

---

# Full Technical Report

[Download Full PDF](/assets/pdfs/fill-station-report.pdf)