---
layout: project
title: MAE 2250 Project
description: Advanced CAD Project
technologies: [Autodesk Fusion]
image: /assets/images/SLF.jpg
---

<style>
.project-image {
  max-width: 525px;
  width: 100%;
  height: auto;
  display: block;
  margin: 20px auto;
  clear: both;
}
</style>

<style>
html {
  scroll-behavior: smooth;
}

h3[id] {
  scroll-margin-top: 100px; /* adjust if you have a navbar */
}
</style>

<h2>Project Overview</h2>
<p>This project focuses on developing a method to aid wineries and grape farms against spotted lanternfly contamination in harvests. It was a semester-long group project required for MAE 2250, Intro to Mechanical Design. It includes three major milestones:</p>

<div class="toc-container">
  <h3>Contents</h3>
  <ul>
    <li><a href="#client-pitch">Client Pitch (ODP3)</a></li>
    <li><a href="#functional-prototype">Functional Prototype (ODP 5)</a></li>
    <li><a href="#client-report">Client Report (ODP 6)</a></li>
  </ul>
</div>

<h3 id="client-pitch">Client Pitch</h3>
<p><strong>Reducing Spotted Lanternfly Contamination During Mechanical Grape Harvest</strong></p>

<p style="font-style: italic;"> By: Lantern Fly Eradication Unit</p>

<p><strong>Problem Statement</strong></p>

<p>During mechanical grape harvest, spotted lantern flies (SLF) remain on the vines and can be collected with the fruit, contaminating loads. Even minimal contamination is unacceptable: as few as 1–2 SLFs (≈1–2 g) can contaminate a 1000 g core sample, triggering shipment rejection.</p>

<p>With deliveries occurring every 10 minutes at roughly 22 tons per load, a single rejected shipment results in substantial product loss, contributing to an estimated $14.3 million of damages across the Lake Erie and Finger Lakes regions in the first three years of infestation.</p>

<p>Current solutions, such as chemical treatments or post-harvest separation, are either ineffective during active harvest, reduce yield, or are operationally inefficient. The challenge is therefore to deter SLF from vines before or during harvest, or to separate them from harvested material, without damaging grape quality or reducing yield.</p>

<br>

<p><strong>Why This Matters to the End-User</strong></p>

<p>Solving this problem would allow vineyards to avoid yield loss from post-harvest washing, reduce SLF contamination in harvested loads, and eliminate the need for additional chemical treatments during a critical harvest window.</p>

<p>By preventing shipment rejections and harvest slowdowns, the solution would preserve grape quality, protect the winery's reputation, and reduce significant economic losses.</p>

<br>

<p><strong>Proposed Directions</strong></p>

<p><em>Smoke Machine Attached to Harvester</em></p>

<p>Attach a smoke (or similar gas) delivery system to the front of the harvester to temporarily deter SLFs from the vines immediately before harvest. The goal is to use a non-lethal substance to clear the vines without relying on pesticides, potentially by rerouting harvester exhaust or using a small gas canister with forward-facing nozzles.</p>

<p>We would prototype with a canister connected to two spray nozzles with an attachment mechanism to the harvester. Key risks/unknowns include whether SLFs will consistently fly away when exposed to smoke or exhaust, whether exposure could affect grape quality, and whether harvesters have sufficient space and power capacity to support the system. These factors would require rigorous prototyping and testing.</p>

<br>

<p><em>Bristles as a Filter</em></p>

<p>Install a system of brush bristles along the inner conveyor of the harvester to mechanically filter SLFs from grapes immediately after harvest. The bristles would comb over the harvested material, allowing grapes and juice to pass while removing SLFs from the harvest.</p>

<p>We would prototype this by designing a brush and running it over grapes with flour or another substance on them. Key risks/unknowns include whether the bristles can reliably filter out SLFs without blocking or damaging grapes, and whether they are durable enough for long-term use. Effective implementation would require experimentation with bristle density and spacing.</p>

<br>

<p><strong>Our Questions</strong></p>

<p><strong>Will SLF consistently disperse when exposed to smoke or exhaust?</strong><br>
Determines whether or not we move forward with the gas or bristle solution.</p>

<p><strong>Are there grape regulatory or flavor concerns regarding smoke or gas exposure?</strong><br>
Clarifies feasibility of the smoke solution, ensuring regulations and flavor aren’t compromised.</p>

<p><strong>Given a known deterrent, how long will it take for SLFs to return to the vines? How long does it take for the harvester to collect the grapes, and will the time of deterrence be long enough?</strong><br>
It is important for us to design the potency, speed, and distribution of our solution.</p>

<p><strong>What are the constraints to the modification of the harvester both internally (for the brush) and externally (for the smoke machine)?</strong><br>
Ensuring the feasibility of attaching a tank to the harvester or adding a bristle filter system.</p>

<h3 id="functional-prototype">Functional Prototype</h3>
<p><td><strong>Design Documentation</strong></td>

<p><strong>MAE2250 Parts List (as of ODP5)</strong></p>
<img src="{{ '/assets/images/MAE2250PartsList.png' | relative_url }}" 
     alt="MAE2250 Parts List" 
     class="project-image">
<p><strong>Assembly Instructions:</strong></p>

<p>1) Cut the 12-inch by 12-inch wooden slab into three equal-width sections. Glued them together with wood glue and clamped them together at the four corners allowed it to rest for 24 hours.</p>

<p>2) Cut the tube down to roughly an 8-inch length, just to make sure there was not too much excess, making the mechanism difficult to use.</p>

<p>3) Cut down the 24-inch length wooden shaft into four 6-inch pieces to prevent motion.</p>

<p>4) Cut one more wooden shaft to roughly 8 inches, and attach it to one gear using tape to use it as a handle.</p>

<p>5) 3D printed gears with CAD from McMaster at the RPL, slightly edited CAD to add a larger hole in the center to decrease the rotational inertia of the mechanism.</p>

<p>6) Drill a 27/64 inch drill bit into the wooden base and glue it down to ensure it is secure. Push two wooden shafts through the two 3D printed gears, but allow the gears to freely rotate. (This was supposed to be done with wooden screws, but our part didn’t come.)</p>

<p>7) Attach the modified 8-inch tubing horizontally to one gear with tape. (This was supposed to be drilled down, but our clamp were a different dimension than intended.)</p>

<p>8) Attach the 8-inch wooden shaft horizontally to the other gear with tape. This will be used for control of the rotational motion of the gears.</p>

<p>9) Drilled a ¼ inch drill bit on each side of the 8-inch wooden shaft. Glue down the two 6-inch wooden shafts into the two holes.</p>

<br>

<p><strong>Illustration</strong></p>

<img src="{{ '/assets/images/ODP5Drawing.jpg' | relative_url }}" 
     alt="MAE2250 Parts List" 
     class="project-image">

<br>

<p><strong>Assembly Instructions:</strong></p>

<p>1) Fasten gears to wooden board with screws so gears are toothed together.</p>
<p>2) Fasten tube for gas dispersion to one gear.</p>
<p>3) Fasten handle to the other gear to allow for controlled rotation.</p>
<p>4) Attach wooden shafts into wooden board to constrain the rotation of the gears.</p>

<br>

<p><strong>Design vs. Drawing Discrepancies:</strong></p>

<p>One major discrepancy is our use of tape as a fastener. This is due to the fact that the clamps we ordered were much larger than we expected, and ended up not being useful for us. This mistake was due to a miscommunication of the tube’s radius and diameter. The team has worked this out, and we have decided to always communicate using diameter due to that being the engineering standard.</p>

<p>Another discrepancy is our lack of wood screws through the center of our gears. This is due to our screw order getting delayed. Although unfortunate, we can prevent this in the future by pushing forward our ordering deadlines on our schedule.</p>

<br>

<p><strong>Design Tests:</strong></p>

<p><strong>Test 1: Rotation Smoothness</strong></p>
<p><strong>Part tested:</strong> Gears</p>
<p><strong>What it tests for:</strong> Whether the handle-driven gears rotate the nozzle smoothly without binding, slipping, or excessive friction.</p>
<p><strong>How we tested it:</strong> Handle was rotated through desired range of motion while observing gear motion and checking for slip, jerky motion, or interference.</p>
<p><strong>Test results:</strong> Before applying constraints to the range of motion, we rotated the gears through 20 full rotations of 360 degrees. Throughout the test, there was no slippage or binding of the gear teeth.</p>
<p><strong>Conclusion for next iteration:</strong> While we did not see any slipping/binding, we noted that the gears must be perfectly placed to achieve that. To provide slight room for error, if we re-fabricate the gears we will increase the gear tooth height by 5mm.</p>

<br>

<p><strong>Test 2: Aiming Range</strong></p>
<p><strong>Part tested:</strong> Tube/Nozzle</p>
<p><strong>What it tests for:</strong> Whether gear system allows tube/nozzle to rotate through motion required to cover desired volumetric space by the gas.</p>
<p><strong>How we tested it:</strong> Handle was turned from one extreme to the other and total angular rotation of the nozzle was measured.</p>
<p><strong>Test results:</strong> The gear system completed 10 full back-and-forth cycles. With the constraints we applied, we achieved a range of motion of 90 degrees. There were 0 instances of slipping or binding by the gear teeth during the test, and the nozzle was able to achieve the range of motion without exhibiting any significant stress.</p>
<p><strong>Conclusion for next iteration:</strong> Our method of constraining the gears was effective. However, to make the design more robust, we will increase the diameter of the wooden cylinder constraints and use an aluminum base instead of wood.</p>

<br>

<p><strong>Test 3: Repeated-Use Durability</strong></p>
<p><strong>Part tested:</strong> Screws/Gears/Wooden Board assembly</p>
<p><strong>What it tests for:</strong> If mechanism maintains functionality after repeated use without loosening, slipping, or increasing friction.</p>
<p><strong>How we tested it:</strong> Handle was cycled at a minimum of 20 times while observing changes in motion smoothness, gear interface, and structural stability.</p>
<p><strong>Test results:</strong> We cycled the gear through 20 full cycles at 20 RPM once the design was fully constructed, including constraints. The design held up with no clear signs of wear and tear.</p>
<p><strong>Conclusion for next iteration:</strong> While our initial design holds up, it is primarily constructed out of cheap wood and tape, meaning that it will lose significant strength over time. For our final design, we will convert the constraint shafts and the base to aluminum. We will also use screws to keep the gears in place instead of wooden sticks.</p>

<br>

<p><strong>Test 4: Tube Stability</strong></p>
<p><strong>Part tested:</strong> Pipe Clamp</p>
<p><strong>What it tests for:</strong> Whether gas tube remains securely attached and doesn’t interfere with nozzle rotation during operation.</p>
<p><strong>How we tested it:</strong> Rotate tube through full range of motion while observing clamps, checking for twisting, sagging, or resistance to rotation.</p>
<p><strong>Test results:</strong> Unfortunately we were not able to directly test this due to our clamp ordering mishap. We however can confidently say that the clamps would hold up in the design, because we taped everything down with painter’s tape, which is significantly weaker. Through all of our previous rotations, roughly 20 full cycles at varying speeds, the tape held up just fine.</p>

<p><strong>Conclusion for next iteration:</strong> We are confident that once we have the correct clamps, they will be strong enough to hold our tube and handle down to demonstrate functionality of our design.</p>

<br>

<p><strong>Test 5: Structural Stability</strong></p>
<p><strong>Part tested:</strong> Wood Mounting Board</p>
<p><strong>What it tests for:</strong> If wooden base remains rigid and maintains gear alignment during use.</p>
<p><strong>How we tested it:</strong> Handle was rotated repeatedly while checking for board flexing, shifting, or misalignment of the gears.</p>
<p><strong>Test results:</strong> We rotated the board through 10 full cycles at 20 RPM while the tube was held down to simulate stress from the harvester, applying a force of 10 Newtons. The wooden base exhibited no signs of flexing/bending, and the gears remained tightly connected with no slippage.</p>

<p><strong>Conclusion for next iteration:</strong> The fact that the base did not flex or shift shows that our design does not have misalignment or place significant stress on the base. That being said, we still plan to use an aluminum base in the next iteration to ensure durability over more extended periods of time.</p>

<br>

<p><strong>Success Criteria:</strong></p>

<p>Our main goal of this iteration is to ensure our gear rotation system for gas dispersion is effective and durable enough to remain undamaged. A successful test should follow all of our outlined design criteria and effectively demonstrate the ability to move our nozzle in a periodic type of motion to achieve better gas dispersion.</p>

<p>After repeated and continuous testing for over 1 minute, where gears spin at least 90 degrees, all gears still spin as intended without interference or skipping.</p>

<p>The gears would need to spin well for the entirety of the harvesting process for multiple harvests. This is important because we would want our solution to work long term for the farmers, so they don’t have to do continuous maintenance of our lanternfly gas dispersal system.</p>

<p>After repeated and continuous testing for over 1 minute, where gears spin at least 90 degrees, all parts remain structurally stable/intact without breaking apart.</p>

<p>Gears that are constrained such that the gas dispersion tube only has an approximate 90-degree range of motion without experiencing significant resistance forces (friction, etc.).</p>

<p>Effective gas dispersion is crucial for our project to work, because it theoretically means the lanternflies would be better dispersed away from the grapes due to a lack of oxygen.</p>
<div style="display: flex !important; flex-direction: row; justify-content: center; align-items: flex-start; gap: 20px; flex-wrap: nowrap;">

  <div style="flex: 0 0 300px;">
    <img src="{{ '/assets/images/ODP5DemoPic1.jpg' | relative_url }}" 
         alt="MAE2250 Demo 1" 
         style="width: 100%; height: auto; display: block;">
  </div>

  <div style="flex: 0 0 300px;">
    <img src="{{ '/assets/images/ODP5DemoPic2.jpg' | relative_url }}" 
         alt="MAE2250 Demo 2" 
         style="width: 100%; height: auto; display: block;">
  </div>

</div>

<p style="margin-bottom: 10px;"></p>

<p><strong>Demo:</strong> Upon spinning the handle, the nozzle rotates with a 90-degree free rotation due to the smooth rotation of the spur gears connected underneath.</p>
</p>

<hr>

<h3 id="client-report">Client Report</h3>

<td><strong>Context and Problem</strong></td>

<p>Spotted Lantern Flies are wreaking havoc on the wine industry by contaminating grape harvests at a devastating scale. To address this issue, our team focused specifically on preventing SLFs from contaminating the harvest by deterring them during grape collection. This stage of the harvesting process represents a critical control point, where even small reductions in SLF presence can significantly reduce the risk of wasting thousands of pounds of grapes.</p>

<p>We chose to focus on pre-harvest and in-process mitigation rather than broader population control because it offers a more immediate and controllable intervention that can be integrated directly into existing harvesting operations. At this point, we believe that seeking to eliminate the SLF population is a much larger issue both in scale and timeline, and we wanted to enable clean harvests now.</p>

<p>Several key constraints shaped our design: it needed to operate in real time alongside harvesting equipment, avoid disrupting current operations, remain low-cost and mechanically simple, and ensure safety for both grapes and workers. These constraints led us to prioritize a solution that targets SLFs just before or during harvest without requiring major changes to existing systems.</p>

<td><strong>Final Prototype & Application</strong></td>

<p>Our team developed a directional nozzle system designed to deter SLFs immediately prior to grape collection. The system uses a gear-driven mechanism connected to a handle, allowing the user to control the orientation of the nozzle to disperse gas across a larger area of the grape vine.</p>

<p>Our device, when placed into commission, will be attached to the front of the grape harvester to dispel gas into the harvesting chamber. When operated, the nozzle will emit lanternfly-deterrent gas intended to disturb and displace SLFs from the vine just before the harvester passes over the grapes and collects them. The oscillating gas distribution system ensures that the most lanternflies possible are repelled away from the grapes immediately before harvest.</p>

<p>In practice, this system would be integrated into existing harvesting equipment and connected to a servo motor. This system would allow an operator to harvest as normal, while gas is automatically dispersed once the system is activated due to the servo motor. This allows SLFs to be removed at the point of harvest without interrupting the harvesting process or requiring significant changes to current operations. The low-hassle implementation of our product is intended to create minimal impact on farmers and keep installation and maintenance costs low.</p>

<p>To test our design, we made a simple mock-up out of metal and 3D printed gears. This system demonstrates the gear mechanism to disperse gas into the grape collection chamber. Although on a final design our system would be actuated by a servo motor, for our final prototype, we determined it sufficient for there to be a handle on one of the gears to mimic the motion the servo motor would provide. Images of the device are provided in the following figures.</p>

<td><strong>Conclusion and Recommendation</strong></td>

<p>Our design so far has been promising and warrants further exploration. Firstly, tests should be conducted to determine a gas that effectively repels lanternflies from the grapes being harvested. It is important to keep in mind when choosing this gas that it could affect harvest quality. It is also critical to consider the availability and cost of the gas to have minimal impact on the farmers implementing this system. Once a gas is decided, field testing can begin with two mechanical systems mounted on either side of the grape harvester, each dispersing the selected gas into the grape harvesting chamber. It is important to keep in mind that in implementation, our mechanical design will be regulated by two servo motors to control the gear actuation and gas dispersal.</p>

<p>We believe our design is feasible due to the proven effectiveness of the mechanical portion. Testing showed that after 50 full rotation cycles, the gears continued to rotate smoothly without slipping or disengaging, the tube remained securely mounted without interfering with motion, and the aluminum base maintained structural stability and gear alignment throughout operation. These results indicate that the core mechanism is reliable enough to withstand repeated use in a harvesting environment and can be integrated into existing equipment with minimal redesign.</p>

<p>Our successful testing, along with the fact that our design is relatively cheap, mechanically reliable, and easy to implement, means that once a gas is fully fleshed out after some further testing, our design is ready for rapid field testing and implementation on grape farms across the Northeast.</p>

<td><strong>Key Testing Results</strong></td>

<p>To evaluate whether this concept is practical for vineyard implementation, we tested the most important mechanical risks: rotational reliability, tubing security, and structural rigidity.</p>

<p>The gear-driven rotation system was tested through 50 full operating cycles across an approximately 90° range of motion. Throughout testing, the gears rotated continuously without observable slipping, disengagement, or excessive friction. This indicates that the mechanism can provide consistent repeated nozzle positioning during harvest operations.</p>

<p>The tube mounting system was also tested through 50 full cycles while monitoring for twisting, sagging, or resistance to motion. The tube remained securely attached and did not interfere with nozzle rotation. This suggests the gas delivery system can remain stable during repeated use and is suitable for future powered actuation.</p>

<p>Finally, the aluminum mounting base was evaluated for structural stability and alignment retention. After repeated cycling, the base showed no visible flexing, shifting, or gear misalignment. This confirms the supporting structure is rigid enough to maintain reliable operation under normal use.</p>

<p>Overall, testing demonstrated that the core mechanical system is low-cost, repeatable, and structurally sound, supporting progression to powered prototypes and field testing.</p>

<td><strong>Prototype & Testing Details</strong></td>

<p>Our prototype was developed as a simple proof of concept to demonstrate the mechanical feasibility of directing deterrent gas across the grape harvesting chamber. The system was constructed using an aluminum mounting base, two large 3D-printed gears, a manual handle, a rubber tube to represent the gas delivery line, and pipe clamps used to secure the tube to the rotating gear.</p>

<p>The aluminum base was used to support the gear shafts and maintain alignment between the driving and driven gears. A handle was attached to the lower gear so that manual rotation could mimic the powered motion that would be produced by a servo motor in a final implementation. As the lower gear rotates, it drives the upper gear, causing the attached tube and nozzle to sweep through the intended range of motion.</p>

<p>The tube was mounted to the upper gear using clamps positioned to keep the tube secure while still allowing smooth rotation. This setup was chosen to represent how a future gas line could be integrated into the system while maintaining directional control of the nozzle. The prototype was intentionally made using simple, low-cost components in order to validate the concept before investing in powered hardware or field-ready materials.</p>

<p>Testing focused on repeated operation of the gear mechanism, tube stability during motion, and structural stability of the base. The handle was rotated repeatedly through the intended range of motion while observing for slipping, binding, interference, or shifting of components. Minor adjustments were made during assembly to improve gear alignment and maintain smooth operation.</p>

<p>In a final design, the manual handle would be replaced by servo motors integrated with the harvesting system, and the prototype materials would be replaced with more durable components suitable for repeated outdoor agricultural use.</p>

<h2>MAE2250 Bill of Materials (Final)</h2>

<style>
table {
  width: 100%;
  border-collapse: collapse;
}

th, td {
  border: 1px solid black;
  padding: 8px;
}

th {
  background-color: #f2f2f2;
}
</style>

<table>
  <thead>
    <tr>
      <th>Item</th>
      <th>Source</th>
      <th>Cost</th>
      <th>Quantity</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Steel Hex Head Screw for Wood Zinc-Plated, M12 Screw Size, 45 mm Long</td>
      <td>McMaster 97498A172</td>
      <td>$9.43</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Vibration-Damping Routing Clamp Zinc-Plated Steel with TPE Rubber Cushion, 7/8" ID</td>
      <td>McMaster 11355T26</td>
      <td>$8.30</td>
      <td>2</td>
    </tr>
    <tr>
      <td>Black-Oxide Alloy Steel Socket Head Screw 10-24 Thread Size, 5/16" Long</td>
      <td>McMaster 91864A032</td>
      <td>$6.12</td>
      <td>1</td>
    </tr>
    <tr>
      <td>(Length=1ft) Multipurpose 6061 Aluminum Bar 3/4" Thick x 4" Wide</td>
      <td>McMaster 8975K233</td>
      <td>$44.04</td>
      <td>1</td>
    </tr>
    <tr>
      <td>(Length=1ft) Air Hose EPDM Rubber, 1/2" ID, 7/8" OD, 300 PSI, Black</td>
      <td>McMaster 5304K28</td>
      <td>$2.56</td>
      <td>1</td>
    </tr>
    <tr>
      <td>(Length=1/2ft) Multipurpose 6061 Aluminum Rod 1/4" Diameter</td>
      <td>McMaster 8974K22</td>
      <td>$1.66</td>
      <td>1</td>
    </tr>
    <tr>
      <td>(Length=1/2ft) Multipurpose 6061 Aluminum Rod 1/2" Diameter</td>
      <td>McMaster 8974K28</td>
      <td>$1.83</td>
      <td>1</td>
    </tr>
    <tr>
      <td>14-1/2 Degree Pressure Angle Plastic Gear Round/Machinable Bore, 12 Pitch, 48 Teeth</td>
      <td>RPL</td>
      <td>$3.90</td>
      <td>2</td>
    </tr>
    <tr>
      <td>Revised Gear with Screw Holes</td>
      <td>RPL</td>
      <td>$2.60</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Revised Gear with Handle</td>
      <td>RPL</td>
      <td>$3.45</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Gas Canister</td>
      <td>RPL</td>
      <td>$17.05</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Plywood 1/4"</td>
      <td>TDS</td>
      <td>$3.00</td>
      <td>1</td>
    </tr>
  </tbody>
</table>

