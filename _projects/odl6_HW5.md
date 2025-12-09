---
layout: project
title: Lifting Frame Mechanism
description: 150cm long and 50cm tall, a rigid bar of a fixed length, 3 pin supports of which two need to be mounted on the ground and a linear actuator to lift max weight
technologies: IPad, My Brain
image: /assets/images/steamshovel.jpg
---

<h3 class="full-width-heading" style="margin-top: 30px; clear: both;">Homework 12 Update - 12/8/25</h3>
<h3 style="color: #333; font-size: 20px; font-weight: bold; margin-top: 15px;">Definition</h3>
Design a planar lifting mechanism that fits entirely within a 150 cm (L) × 50 cm (H) rectangular design space and uses:
- One rigid bar (fixed length)
- Three pin supports (exactly two must be ground-mounted)
- One linear actuator (from the provided IMA catalog), to lift the maximum possible weight to the highest possible height. Assume all links and supports are rigid and frictionless for the Step 1 analysis.

<h3 style="color: #333; font-size: 20px; font-weight: bold; margin-top: 15px;">Constraints</h3>
- Envelope: everything (all poses) must remain inside 150 × 50 cm.
- Supports: exactly two ground pins; the third pin is on the moving bar.
- Single rigid bar (no telescoping).
- One linear actuator (no cables, pulleys, or extra links).
- Pins are ideal; members and actuator are axially rigid (Step 1 only).
- Vertical lift is measured by the vertical displacement of the load hook pinned to the end of the bar.
- Avoid over-center lockup unless reachable inside the envelope and retractable.

<h3 style="color: #333; font-size: 20px; font-weight: bold; margin-top: 15px;">Objectives</h3>
- Max vertical lift of the load hook within the 50 cm height limit.
- Max load capacity for a chosen actuator (maximize mechanical advantage where needed).
- Feasible stroke and clearances for the selected actuator.
- Simple, manufacturable geometry (single bar; 3 pins total; no side-loads on actuator).

<h3 style="color: #333; font-size: 20px; font-weight: bold; margin-top: 15px;">Design Degrees of Freedom</h3>
- Bar length L (fixed for Step 1).
- Ground-pin spacing A-B (both on the ground line).
- Actuator attach location on bar a (distance from A to pin D)
- Initial and final bar angles θ<sub>start</sub>,θ<sub>end</sub> set by stroke and clearances).
- Actuator package orientation (which side of the bar it pushes, mount style at B/D).
- Exact placement of the load hook (we’ll use the bar tip at C for maximum reach).

<h3 style="color: #333; font-size: 20px; font-weight: bold; margin-top: 15px;">Static Analysis</h3>
You get the biggest actuator lever arm if you attach it as far from the pivot as possible, so, I put it a the other end of the bar. I located the optimal actuator ground pin location by placing it perpendicular to the bar at the minimum stroke. In doing so, the actuator’s entire force contributes to torque at the start, giving the best worst-case leverage. I made the bar length 50cm to fit inside the design constraint but result in maximum lift.

<h3 style="color: #333; font-size: 20px; font-weight: bold; margin-top: 15px;">Design</h3>
<img src="/assets/images/liftmech1.jpeg" width=600px>


<!-- Separator between sections -->

<h3 style="color: #333; font-weight: bold; margin-top: 30px;">Homework 5 - Original</h3>
I designed this mechanism to lift the maximum weight possible in a 150cm by 50cm spade with 3 pin supports, 2 of which are mounted on the ground and lifted by a linear actuator. I chose to use the IMA55-RN05 linear actuator with peak thrust ≈ 23,900 lbf (106 kN) and stroke options up to ~18 in (457 mm). The ground pins are located 120cm apart, and the rigid bar is 50cm long for maximum height availability. 

<img src="/assets/images/image_HW5.jpg" width=300px>

git add .
git commit -m "<Commit Edit>"
git push origin main
