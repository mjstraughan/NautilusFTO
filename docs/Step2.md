---
title: Centers - Nautilus
description: Centers guide for the Nautilus FTO method
---

# Centers

In the next step, solve the three large centers to the right of the first block. These are the F, BR, and U centers. Only two need to be solved and the third center will be automatically solved. The move set is now reduced to U, R, r and slice turns. This will feel familiar to those experienced with the center solving process of big cubes.

<div class="applet-grid-nowrap">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IDIDII,CENTERS:DIIII----D----III-DDDDDI,EDGES:-------D--DD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

## First Center

Attach triangles and edges to form a half center. In the first of the following applets, a triangle from the bottom is attached to the edge on the upper layer then a second edge is added and the half center is moved to its correct position. In the second applet, a triangle and edge pair is created, the final triangle is attached, and the half center is attached to the first half center.

<div class="solve-row">

    <div class="solve-container">

        <twisty-player
            id="fto-player-1"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIII-I-IIIIIIII-----I,EDGES:-IIIII--II--"
            experimental-setup-alg="LBLv r' U R U R' U R'"
            alg="R . // Pair triangle with edge
            U' R U' R' . // Add edge to pair
            U' r // Position half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

        <twisty-alg-viewer
            for="fto-player-1"
        ></twisty-alg-viewer>

    </div>

    <div class="solve-container">

        <twisty-player
            id="fto-player-2"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-I-IIIIII-----I,EDGES:-III-I--II--"
            experimental-setup-alg="LBLv R' U R' U R U' R'"
            alg="R U R' . // Pair triangle with edge
            U' R . // Add triangle to pair
            U' R // Position half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

        <twisty-alg-viewer
            for="fto-player-2"
        ></twisty-alg-viewer>

    </div>
</div>

## Second Center

Follow the same process to solve the second center. In the first of the following applets, the triangle on the bottom is attached to an edge, then the other edge is attached and the half center is positioned. In the second applet, two triangles are attached to the final edge and the half center is solved. This automatically solves the U layer center. Be careful during this step to not break the first center that was built.

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-3"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-I--IIIII-----I,EDGES:-III-I------"
            experimental-setup-alg="LBLv 2R U R U r' U' R U' R'"
            alg="R U R' . // Pair triangle with edge
            U r U' R' U' 2R' // Add edge to pair and solve half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-3"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-4"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R' U R U' R'"
            alg="R U R' . // Move triangle to first two layers
            U' R U R' // Attach triangle to pair and solve"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-4"></twisty-alg-viewer>
  </div>

</div>

## Freeform Center Strategy

It can be restrictive to always solve the back center then the front center. This is where freeform center solving can often yield better results. For example, the front center can be solved and placed in the back. Then solve the back center on the U layer and make the final centers adjustment. It also isn't necessary to always focus on the front and back centers. The U center can be one of the two that are built during this process, leading to either the front or back center being the one that is automatically solved in the end.

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-5"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIIIII--I--IIII-----I,EDGES:II-IIII-----"
            experimental-setup-alg="LBLv r' R' U R U R' r' U' R"
            alg="R' U r . // Half center
            R U' R' U' R // Create and add other half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-5"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-6"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv r' R U' R' U r U r' U R U' R'"
            alg="R U R' U r U' r' R U R' . // Build second center
            r // Align all centers"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-6"></twisty-alg-viewer>
  </div>

</div>

## Half Center Strategy

Instead of building whole centers one at a time, another strategy is to build half centers from multiple centers then attach the half centers together. In the applets, the half centers of the left side of the front and back are solved, then the half centers of the right side are solved.

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-7"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIII-I-II-IIIII-----I,EDGES:-IIIII------"
            experimental-setup-alg="LBLv r U R' U r' r' U R'"
            alg="R U' r . // Back half center
            r U' R U' r' // Front half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-7"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-8"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U R U' R' R' U R"
            alg="R' U' R . // Back half center
            R U R' U' R U' R' // Front half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-8"></twisty-alg-viewer>
  </div>

</div>

## Freeform Half Center Strategy

The half center strategy can combined with the freeform center building strategy to create pseudo half centers. Using this strategy, any half centers can be built and grouped while working on other half centers that will all eventually be correctly aligned. The same automatic third center solving property applies, except in this case it is thought of as the final two half centers will be automatically solved. In the first applet, the left halves of the front and back centers are solved, then the right half of the front center is placed in the back position, and finally the right half of the back center is built and solved. In the second example, The left half of the front center and the right half of the back center are placed in the back, and the final two half centers are built and solved.

### Example 1

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-9"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIII-I-II-IIIII-----I,EDGES:-IIIII------"
            experimental-setup-alg="LBLv r U R' U r' r' U R'"
            alg="R U' r . // Back half center
            r U' R U' r' // Front half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-9"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-10"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R' U R U R' U' R' U R"
            alg="R' U' R . // Front half center in back
            U R U' R' U' R // Build back half center and solve"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-10"></twisty-alg-viewer>
  </div>

</div>

### Example 2

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-11"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-III-I--IIIII-----I,EDGES:IIII-II-----"
            experimental-setup-alg="LBLv 2R' R' U' R r' U R'"
            alg="R U' r . // Front half center in back
            R' U R // Back half center"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-11"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-12"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv r' R' U' R' U' r U r' U R U' R'"
            alg="R U R' U' r U' r' U R U . // Build remaining two half centers
            R r  // Align half centers"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-12"></twisty-alg-viewer>
  </div>

</div>

## Edge Order Correction

Sometimes when solving the last two centers the center you are currently working on will have two edges in the incorrect order. Instead of using a long sequence of turns to correct the edge order then finish adding the last three pieces, you can easily solve the last two centers at once using a simple technique. During the final three move R U R' insert that would form the center with the incorrect three edge order, instead adjust the two U layer pieces and the center then use an alternate three move insert.

<div class="solve-row">
    <div class="solve-container">

        <twisty-player
            id="fto-player-13"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII---------III------I,EDGES:------------"
            experimental-setup-alg="LBLv r R' U R U' r' U'"
            alg="U r U R' U' R r'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

        <twisty-alg-viewer
        for="fto-player-13"
        ></twisty-alg-viewer>
    </div>
</div>

## Useful Second Center Solutions

Below are solutions for when three pieces of the second center remain. These aren't intended to be memorized. Instead, learn how each solution works.

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-14"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R'"
            alg="R U R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-14"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-15"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R'"
            alg="R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-15"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-16"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R' U' R U' R'"
            alg="R U R' U R U R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-16"></twisty-alg-viewer>
  </div>

</div>

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-17"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U R U' R'"
            alg="R U R' U' R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-17"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-18"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R' U R U R'"
            alg="R U' R' U' R U R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-18"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-19"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R' U R U' R'"
            alg="R U R' U' R U R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-19"></twisty-alg-viewer>
  </div>

</div>

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-20"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U' R U R'"
            alg="R U' R' U R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-20"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-21"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U' R U' R'"
            alg="R U R' U R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-21"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-22"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R' U' R U R'"
            alg="R U' R' U R U R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-22"></twisty-alg-viewer>
  </div>

</div>

<div class="solve-row">

  <div class="solve-container">
        <twisty-player
            id="fto-player-23"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U' R U' R' U' R U R'"
            alg="R U' R' U R U R' U R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-23"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-24"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U R U' R' U R U' R'"
            alg="R U R' U' R U R' U' R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-24"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
        <twisty-player
            id="fto-player-25"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U' R' U R U R' U' R U R'"
            alg="R U' R' U R U' R' U' R U R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    <twisty-alg-viewer for="fto-player-25"></twisty-alg-viewer>
  </div>

</div>

<div class="solve-row">
    <div class="solve-container">

        <twisty-player
            id="fto-player-26"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIII-I-I-----IIII-----I,EDGES:-I-I-I------"
            experimental-setup-alg="LBLv R U R' U R U' R' U' R U R'"
            alg="R U' R' U R U R' U' R U' R'"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

        <twisty-alg-viewer
        for="fto-player-26"
        ></twisty-alg-viewer>
    </div>
</div>