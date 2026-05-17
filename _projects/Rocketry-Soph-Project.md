---
layout: project
order: 1
title: Rocketry Project 2025-2026
description: Year long project focused on insulating and dust-proofing launch-critical ground station. 
technologies: [SolidWorks, 3D Printing]
image: /assets/images/CRT-Logo.png
---


# Fill Station Electronics Enclosure

---

## Overview

This project focused on the structural and thermal design of an electronics enclosure for a rocket fill station system. The enclosure was designed to:

- Securely mount electrical systems
- Prevent overheating in desert competition environments
- Minimize dust intrusion
- Maintain accessibility for wiring and maintenance

---

# Dust Cover Images

<div class="image-grid">

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/DustCover1.png' | relative_url }}">
    <figcaption>Dust Cover 1</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/DustCover2.png' | relative_url }}">
    <figcaption>Dust Cover 2</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/DustCover3.png' | relative_url }}">
    <figcaption>Dust Cover 3</figcaption>
  </figure>

</div>

---

# Board Mount Images

<div class="image-grid">

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/PowerBoardMount.png' | relative_url }}">
    <figcaption>Power Board Mount</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/SenseBoardMount.png' | relative_url }}">
    <figcaption>Sense Board Mount</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/SKAM-HatMount.png' | relative_url }}">
    <figcaption>SKAM-Hat Mount</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/SKAMBoardMount.png' | relative_url }}">
    <figcaption>SKAM Board Mount</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/IgnitorBoardMount.png' | relative_url }}">
    <figcaption>Ignitor Board Mount</figcaption>
  </figure>

  <figure>
    <img class="uniform-image" src="{{ '/assets/images/BallValveBoardMount.png' | relative_url }}">
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

<table style="width:100%; border-collapse:collapse; border:2px solid #333; margin:25px 0; font-family:Arial, sans-serif; font-size:0.95rem;">

  <thead>
    <tr>
      <th style="border:1px solid #333; padding:12px 15px; background:#eaeaea; text-align:center;">
        Requirement
      </th>
      <th style="border:1px solid #333; padding:12px 15px; background:#eaeaea; text-align:center;">
        Reasoning
      </th>
      <th style="border:1px solid #333; padding:12px 15px; background:#eaeaea; text-align:center;">
        Solution
      </th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Easy board installation</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Ease of assembly</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Heat-set inserts and screws</td>
    </tr>

    <tr>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">External port access</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Accessibility</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Wire pass-through dust covers</td>
    </tr>

    <tr>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Secure mounting</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Transport safety</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">VHB + inserts</td>
    </tr>

    <tr>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Fit inside enclosure</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">System integration</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">CAD-constrained layout</td>
    </tr>

    <tr>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Minimize dust entry</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Prevent shorts</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">RTV-sealed openings</td>
    </tr>

    <tr>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Thermal mitigation</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">Prevent overheating</td>
      <td style="border:1px solid #333; padding:12px 15px; text-align:center;">White paint + raised stand</td>
    </tr>
  </tbody>

</table>


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