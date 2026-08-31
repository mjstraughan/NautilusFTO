---
title: Introduction - Nautilus
description: Introduction to the Nautilus method for FTO
---

# **Introduction**

<div class="applet-grid-nowrap">

<twisty-player
    puzzle="fto"
    experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIIIII-IIIIIIII-----I,EDGES:IIIIIII-II--"
experimental-setup-alg="LBLv"
experimental-setup-anchor="end"
    background="none"
control-panel="none"
  ></twisty-player>

<twisty-player
    puzzle="fto"
    experimental-stickering-mask-orbits="C4RNER:IDIDII,CENTERS:DIIII----D----III-DDDDDI,EDGES:-------D--DD"
experimental-setup-alg="LBLv"
experimental-setup-anchor="end"
    background="none"
control-panel="none"
  ></twisty-player>

<twisty-player
    puzzle="fto"
    experimental-stickering-mask-orbits="C4RNER:IDIDI-,CENTERS:DI-IIDDDDDDDDDIIIDDDDDD-,EDGES:DDDDDDDDDDDD"
experimental-setup-alg="LBLv"
experimental-setup-anchor="end"
    background="none"
control-panel="none"
  ></twisty-player>

<twisty-player
    puzzle="fto"
    experimental-stickering-mask-orbits="C4RNER:-D-D-D,CENTERS:D-D--DDDDDDDDD---DDDDDDD,EDGES:DDDDDDDDDDDD"
experimental-setup-alg="LBLv"
experimental-setup-anchor="end"
    background="none"
control-panel="none"
  ></twisty-player>

</div>

Nautilus is a Face Turning Octahedron (FTO) speedsolving method designed for ergonomics, efficiency, and automation. The first two steps of the method intuitively solve pieces in such a way that blind spots are minimized and look ahead is maximized. The final two steps are automated through the use of algorithms. Recognition is simple thanks to all pieces being in view.

## Advantages

**Algorithm based ending:** The final steps either use memorized algorithms with drilled ergonomics, or are automatic due to the simplicity. This removes any thinking time and ensures that the best and fastest solutions are always used, as opposed to intuitive solving where the solver may not always find the most ergonomic or shortest solutions.

**Easy recognition:** The last layer step in Nautilus requires checking just the side stickers of the last layer, similar to two sided PLL recognition on 3x3. Some endings in other methods require checking multiple faces and layers to know the case.

**Easy to understand:** The final steps of the method use algorithms. Plus for beginners there are just six algorithms to learn for the basic method. So there is no need to learn and practice an intuitive solution that may be difficult to understand.

**Ergonomic:** After the first block, the center solving step involves very fast and easy turning in the U R r move set. The final two steps are designed around freedom of movement and use algorithms that have been highly optimized for speed solving.

**Efficient:** The overall method is highly efficient thanks to the first two steps reducing to a state that allows for an easy to learn three step finish, or a more advanced two step finish.

**Easy memorization:** Last layer algorithms feel unique, making them easy to memorize. Some FTO methods involve heavy use of sledges and hedges, which are preset 4 move sequences throughout the algorithms. This can make it difficult to differentiate the cases during memorization.

**Expandable:** The final steps have potential for advancements. The last triple can likely be easily integrated into the centers step, or the last layer can be influenced while solving the last triple (similar to ZBLS), or the number of pieces involved in the last triple step can be increased to solve more at once in a single algorithm.

## Example Solve

<div class="solve-row">
   <div class="solve-container">

    <twisty-player
        id="fto-player"
        puzzle="fto"
        experimental-setup-alg="LBLv L D R' B L' B R D U' L' B' R U B U' B D' R L' D' F' BR' R' L U B'"
        alg="Uv U' BL L D L' R U' L' U L // Arrow block
        U' B U' B' // Finish first block&#10;U R' U' r' U R' U' R U R' // First center
        U' r' U' R U' R' U' R U R' U r' // Second center
        U R BR' br U BR U' br' R' // Last triple
        br U BR' U' br' F BR F' // L6X
        br' R U' R' br U br' R U' R' br // Last 3 Corners"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

    <twisty-alg-viewer id="fto-alg-viewer" for="fto-player"></twisty-alg-viewer>
  </div>
</div>