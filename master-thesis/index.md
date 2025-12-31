---
layout: default
title: Master Thesis
---

This thesis builds a deployable pipeline for object goal navigation on Boston Dynamics Spot in known indoor environments. A short teleoperated run creates a 2D occupancy map and a compact semantic database of confirmed objects. Later, a user selects a mapped object and the system generates a safe standoff goal and sends it to Nav2 for planning and control.

## Semantic mapping demo
RGB D detections are projected into the map frame through TF and fused over time to keep only confirmed, static object instances. The result is exported as a small YAML database that stays easy to inspect and debug.

<div class="video">
  <iframe
    src="https://www.youtube.com/embed/F4q-SN-NFhI"
    title="Semantic mapping"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen></iframe>
</div>

## Voice based object goal navigation demo
A speech frontend transcribes short commands with a local Whisper model, then a lightweight language step selects a target from the saved semantic database. The same goal generator produces an offset and facing NavigateToPose goal for Nav2.

<div class="video">
  <iframe
    src="https://www.youtube.com/embed/cdXH4_lS0m8"
    title="Voice based object goal navigation"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen></iframe>
</div>
