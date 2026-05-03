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
  <p>Content here</p>
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
