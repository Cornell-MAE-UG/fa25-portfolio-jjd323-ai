---
layout: project
order: 1
title: Rocketry Project 2025-2026
description: Year long project focused on insulating and dust-proofing launch-critical ground station. 
technologies: [SolidWorks, 3D Printing, Thermodynamic Analysis]
image: /assets/images/CRT-Logo.png
---


# Overview

This project focused on the structural and thermal design of an electronics enclosure for a rocket fill station ground control system used in a desert competition environment. The system integrates launch-critical electronics within a rugged SKB enclosure.

The design prioritizes secure component mounting, thermal protection against extreme desert conditions, dust mitigation, and maintainable access for wiring and electrical system servicing and iterating.

This was a year long-project, completed for Cornell Rocketry's 2025-2026 launch vehicle, Valkyrie.
 
---

# Full Report Download

A brief summary of the project is included on this webpage. The full report is availble to download here.

<a href="{{ '/assets/pdfs/Rocketry-Report-Soph.pdf' | relative_url }}"
   style="display:inline-block; padding:10px 16px; border:2px solid #000; text-decoration:none; margin:10px 0;">
  📄 Download Full Report (PDF)
</a>

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

<table style="width:100%; border-collapse:collapse; border:2px solid #000; margin:25px 0; font-family:Open Sans, Montserrat,Helvetica Neue sans-serif; font-size:0.95rem;">

  <thead>
    <tr>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Requirement
      </th>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Reasoning
      </th>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Solution
      </th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Easy board installation</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Ease of assembly</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Heat-set inserts and screws</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">External port access</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Accessibility</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Wire pass-through dust covers</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Secure mounting</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Transport safety</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">VHB + inserts</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Fit inside enclosure</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">System integration</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">CAD-constrained layout</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Minimize dust entry</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Prevent shorts</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">RTV-sealed openings</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Thermal mitigation</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Prevent overheating</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">White paint + raised stand</td>
    </tr>
  </tbody>

</table>

---

# Thermal Analysis

The dominant heat source for the enclosure was determined to be solar radiation.

The enclosure temperature was modeled using an energy balance derived from the First Law of Thermodynamics:

$\alpha G A_{\text{sun}} - \varepsilon \sigma A_{\text{box}} ( T_s^4 - T_{\text{air}}^4 ) - h A_{\text{box}} ( T_s - T_{\text{air}} ) = 0$

<table style="width:100%; border-collapse:collapse; border:2px solid #000; margin:25px 0; font-family:Open Sans, Montserrat, Helvetica Neue, sans-serif; font-size:0.95rem;">

  <thead>
    <tr>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Variable
      </th>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Meaning
      </th>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Units
      </th>
    </tr>
  </thead>

  <tbody>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$\alpha$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Solar absorptivity</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">(dimensionless)</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$G$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Solar irradiance</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">W/m²</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$A_{sun}$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Projected solar area</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">m²</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$\varepsilon$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Surface emissivity</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">(dimensionless)</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$\sigma$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Stefan–Boltzmann constant</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">W/m²·K⁴</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$T_s$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Surface temperature</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">K or °F</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$T_{air}$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Ambient temperature</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">K or °F</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$h$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Convective heat transfer coefficient</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">W/m²·K</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$A_{box}$</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Exposed surface area</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">m²</td>
    </tr>

  </tbody>

</table>

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

# Other Design Options

Multiple other design options were looked into for thermal mitigation, but were ultimately scrapped. 

<h3 style="font-style: italic;">Water Cooling System</h3>

A water-cooling system was considered as a potential thermal management solution for the electronics enclosure. This approach was ultimately not selected because it does not address the dominant heat load, which is solar radiation entering the enclosure, and instead primarily targets internal heat generation from the electronics, which was estimated to be a secondary contributor. In addition, a liquid-based cooling system would significantly increase system cost and complexity, while introducing a risk of leakage that could result in electrical failure or short-circuiting of sensitive components. Due to these constraints, a detailed thermal analysis of this option was not pursued.

<h3 style="font-style: italic;">Reflective Heat Shield</h3>
The option of a reflective heat shield was also investigated. Compared to a water-cooling system, this approach more directly reduces the dominant heat input from solar radiation and is significantly lower in cost. However, its overall cost was found to be comparable to that of a glossy white paint finish, so a thermal analysis was performed to compare performance.

For a reflective heat shield:

$$
\alpha \approx 0.1
$$

$$
\varepsilon \approx 0.3
$$

The predicted maximum temperature (using the previously derived energy balance model) was:

$$
T_{\max} = 120^\circ F \approx 49^\circ C
$$

This result is thermodynamically similar to the glossy white paint case, indicating minimal thermal benefit from the change in surface properties alone. As a result, this option was not selected. The primary drawback was implementation reliability: the design would require adhesive-backed reflective sheets applied to the enclosure surface, which would likely degrade under shipping loads and prolonged exposure to harsh field conditions. In contrast, paint provides a more durable and integrated surface treatment. For these reasons, the reflective heat shield concept was not pursued further.

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

<table style="width:100%; border-collapse:collapse; border:2px solid #000; margin:25px 0; font-family:Open Sans, Montserrat, Helvetica Neue, sans-serif; font-size:0.95rem;">

  <thead>
    <tr>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Item
      </th>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Supplier
      </th>
      <th style="border:1px solid #000; padding:12px 15px; background:#f7f8fa; text-align:center;">
        Cost
      </th>
    </tr>
  </thead>

  <tbody>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">VHB Tape</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Amazon</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$22.46</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">White Paint</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Home Depot</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$50.94</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Heat-set Inserts</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">McMaster</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$15.22</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Plastic Primer</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">McMaster</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$14.98</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Screws</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">McMaster</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$7.69</td>
    </tr>

    <tr>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">Plastic Washers</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">McMaster</td>
      <td style="border:1px solid #000; padding:12px 15px; text-align:center;">$12.12</td>
    </tr>

  </tbody>

</table>

---

# Full Technical Report

[Download Full PDF]({{ '/assets/pdfs/Rocketry-Report-Soph.pdf' | relative_url }})