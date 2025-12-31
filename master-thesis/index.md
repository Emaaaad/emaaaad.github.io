---
layout: default
title: Master Thesis
---

<div class="card">
  <h2 style="margin-top:0">Semantic Object-Goal Navigation on a Quadruped</h2>
  <p style="margin-bottom:0">
    Two-stage workflow. First, a short teleop run builds a 2D map and saves confirmed object instances into a small semantic database.
    Then the robot localizes on the saved map and navigates to a selected object with a safe standoff goal using Nav2.
  <p style="margin-top:12px; margin-bottom:0">
    <a class="btn" href="{{ '/assets/thesis.pdf' | relative_url }}" target="_blank" rel="noopener">Download thesis PDF</a>
  </p>
  </p>
</div>

<div class="section">
  <div class="card">
    <h3 style="margin-top:0">Semantic mapping demo</h3>
    <p style="margin-bottom:0">
      RGB-D detections are projected into the map frame, fused over time, and stored only when they are stable enough to be trusted.
    </p>
  </div>

  <div class="video">
    <iframe
      src="https://www.youtube-nocookie.com/embed/F4q-SN-NFhI"
      title="Semantic mapping"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen></iframe>
  </div>
</div>

<div class="section">
  <div class="card">
    <h3 style="margin-top:0">Voice-based object-goal navigation demo</h3>
    <p style="margin-bottom:0">
      A voice command selects a target from the saved semantic database, then the system sends a standard NavigateToPose goal to Nav2.
    </p>
  </div>

  <div class="video">
    <iframe
      src="https://www.youtube-nocookie.com/embed/cdXH4_lS0m8"
      title="Voice based object goal navigation"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen></iframe>
  </div>
</div>

