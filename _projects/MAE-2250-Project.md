---
layout: project
title: MAE 2250 Project
description: Advanced CAD Project
technologies: [Autodesk Fusion]
image: /assets/images/SLF.jpg
---

<button class="accordion">Client Pitch</button>
<div class="panel">
  <p>Content here</p>
</div>

<button class="accordion">Functional Prototype</button>
<div class="panel">
  <p>Content here</p>
</div>

<button class="accordion">Client Report</button>
<div class="panel">
  <p>Context & Problem 

Spotted Lantern Flies are wreaking havoc on the wine industry by contaminating grape harvests at a devastating scale. To address this issue, our team focused specifically on preventing SLFs from contaminating the harvest by deterring them during grape collection. This stage of the harvesting process represents a critical control point, where even small reductions in SLF presence can significantly reduce the risk of wasting thousands of pounds of grapes.

We chose to focus on pre-harvest and in-process mitigation rather than broader population control because it offers a more immediate and controllable intervention that can be integrated directly into existing harvesting operations. At this point, we believe that seeking to eliminate the SLF population is a much larger issue both in scale and timeline, and we wanted to enable clean harvests now.

Several key constraints shaped our design: it needed to operate in real time alongside harvesting equipment, avoid disrupting current operations, remain low-cost and mechanically simple, and ensure safety for both grapes and workers. These constraints led us to prioritize a solution that targets SLFs just before or during harvest without requiring major changes to existing systems.

Final Prototype & Application
Our team developed a directional nozzle system designed to deter SLFs immediately prior to grape collection. The system uses a gear-driven mechanism connected to a handle, allowing the user to control the orientation of the nozzle to disperse gas across a larger area of the grape vine. 
Our device, when placed into commission, will be attached to the front of the grape harvester to dispel gas into the harvesting chamber. When operated, the nozzle will emit lanternfly-deterrent gas intended to disturb and displace SLFs from the vine just before the harvester passes over the grapes and collects them. The oscillating gas distribution system ensures that the most lanternflies possible are repelled away from the grapes immediately before harvest.
In practice, this system would be integrated into existing harvesting equipment and connected to a servo motor. This system would allow an operator to harvest as normal, while gas is automatically dispersed once the system is activated due to the servo motor. This allows SLFs to be removed at the point of harvest without interrupting the harvesting process or requiring significant changes to current operations. The low-hassle implementation of our product is intended to create minimal impact on farmers and keep installation and maintenance costs low. 
To test our design, we made a simple mock-up out of metal and 3D printed gears. This system demonstrates the gear mechanism to disperse gas into the grape collection chamber. Although on a final design our system would be actuated by a servo motor, for our final prototype, we determined it sufficient for there to be a handle on one of the gears to mimic the motion the servo motor would provide. Images of the device are provided in the following figures. 
Conclusion & Recommendation

Our design so far has been promising and warrants further exploration. Firstly, tests should be conducted to determine a gas that effectively repels lanternflies from the grapes being harvested. It is important to keep in mind when choosing this gas that it could affect harvest quality. It is also critical to consider the availability and cost of the gas to have minimal impact on the farmers implementing this system. Once a gas is decided, field testing can begin with two mechanical systems mounted on either side of the grape harvester, each dispersing the selected gas into the grape harvesting chamber. It is important to keep in mind that in implementation, our mechanical design will be regulated by two servo motors to control the gear actuation and gas dispersal. 

We believe our design is feasible due to the proven effectiveness of the mechanical portion. Testing showed that after 50 full rotation cycles, the gears continued to rotate smoothly without slipping or disengaging, the tube remained securely mounted without interfering with motion, and the aluminum base maintained structural stability and gear alignment throughout operation. These results indicate that the core mechanism is reliable enough to withstand repeated use in a harvesting environment and can be integrated into existing equipment with minimal redesign.

Our successful testing, along with the fact that our design is relatively cheap, mechanically reliable, and easy to implement, means that once a gas is fully fleshed out after some further testing, our design is ready for rapid field testing and implementation on grape farms across the Northeast.

Key Testing Results

To evaluate whether this concept is practical for vineyard implementation, we tested the most important mechanical risks: rotational reliability, tubing security, and structural rigidity.

The gear-driven rotation system was tested through 50 full operating cycles across an approximately 90° range of motion. Throughout testing, the gears rotated continuously without observable slipping, disengagement, or excessive friction. This indicates that the mechanism can provide consistent repeated nozzle positioning during harvest operations.

The tube mounting system was also tested through 50 full cycles while monitoring for twisting, sagging, or resistance to motion. The tube remained securely attached and did not interfere with nozzle rotation. This suggests the gas delivery system can remain stable during repeated use and is suitable for future powered actuation.

Finally, the aluminum mounting base was evaluated for structural stability and alignment retention. After repeated cycling, the base showed no visible flexing, shifting, or gear misalignment. This confirms the supporting structure is rigid enough to maintain reliable operation under normal use.

Overall, testing demonstrated that the core mechanical system is low-cost, repeatable, and structurally sound, supporting progression to powered prototypes and field testing.

Prototype and Testing Details

Our prototype was developed as a simple proof of concept to demonstrate the mechanical feasibility of directing deterrent gas across the grape harvesting chamber. The system was constructed using an aluminum mounting base, two large 3D-printed gears, a manual handle, a rubber tube to represent the gas delivery line, and pipe clamps used to secure the tube to the rotating gear.

The aluminum base was used to support the gear shafts and maintain alignment between the driving and driven gears. A handle was attached to the lower gear so that manual rotation could mimic the powered motion that would be produced by a servo motor in a final implementation. As the lower gear rotates, it drives the upper gear, causing the attached tube and nozzle to sweep through the intended range of motion.

The tube was mounted to the upper gear using clamps positioned to keep the tube secure while still allowing smooth rotation. This setup was chosen to represent how a future gas line could be integrated into the system while maintaining directional control of the nozzle. The prototype was intentionally made using simple, low-cost components in order to validate the concept before investing in powered hardware or field-ready materials.

Testing focused on repeated operation of the gear mechanism, tube stability during motion, and structural stability of the base. The handle was rotated repeatedly through the intended range of motion while observing for slipping, binding, interference, or shifting of components. Minor adjustments were made during assembly to improve gear alignment and maintain smooth operation.

In a final design, the manual handle would be replaced by servo motors integrated with the harvesting system, and the prototype materials would be replaced with more durable components suitable for repeated outdoor agricultural use.
</p>
</div>


<script>
var acc = document.getElementsByClassName("accordion");
for (let i = 0; i < acc.length; i++) {
  acc[i].onclick = function() {
    this.classList.toggle("active");
    let panel = this.nextElementSibling;
    panel.style.display = panel.style.display === "block" ? "none" : "block";
  };
}
</script>
