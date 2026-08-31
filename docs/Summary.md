---
title: Summary - Nautilus
description: Summary and additional ideas for the Nautilus FTO method
---

# Summary

<div class="centered-link-wrapper">
    <a href="https://discord.gg/GJB2ER2Q3M" class="custom-styled-link" target="_blank" rel="noopener noreferrer">Join My Discord Server</a>
</div>

<div class="centered-link-wrapper">
    <a href="https://sites.google.com/site/athefre" class="custom-styled-link" target="_blank" rel="noopener noreferrer">My Main Development Website</a>
</div>

The Nautilus method is developed by Michael James Straughan (Athefre) in coordination with several others. Liam Highducheck, Vincent Trang, Malte Ihlefeld, Ryan Hudgens, and mrmangohands have all contributed step ideas, algorithms, and general thoughts that have refined Nautilus. Several others have also contributed algorithms. crystalcuber has been pivotal in ensuring that Nautilus has high quality images, with his development of an <a href="https://fto-image-gen.netlify.app/">image generator</a>. Join my Discord server above to become part of the community.

Why is it called Nautilus? Nautilus started as a method for 3x3. That method solves F2L minus a 1x2x2 block, called LXS or the LXSLL state. This allows for <U, r U r'> turning. Eventually <U, r U r'> and the general shape idea became a concept of its own that easily adapts to other puzzles. As for FTO, the main steps of Nautilus taught on the website correspond with the 3x3 Nautilus method because the step 1 FB and step 2 large centers steps create a similar shape to the LXSLL state, leaving just a "front" pair and a last layer to be solved. Within the "Future of F2L" section on this page there is an idea for an EIF version of Nautilus that does FB then a 2x2x2 triangle block within the F2L, also leaving the FTO in the <U, r U r'> state.

Puzzle community member Fuvash has written a tutorial for the Japanese community. It is very detailed, providing individual articles for each step of the method, including images and numerous example solves for each step. The tutorial even goes in depth into a color neutrality technique and teaches the advanced last slot building technique mentioned below on this page.

<div class="centered-link-wrapper">
    <a href="https://note.com/fuvash/m/maf9b83914c39" class="custom-styled-link" target="_blank" rel="noopener noreferrer">Nautilus Guide in Japanese</a>
</div>

## Future of F2L

The future of Nautilus solving may involve expanding F2L to include more ways of solving, similar to CFOP's trend toward more blockbuilding. Below are a few ideas.

### Stripe

A small change from the current Nautilus F2L style is to solve a stripe next to the first block. This solves the left half of the F and BR centers. Then solve the remainder of the F2L.

1. FB
2. Stripe - Solve the slice of the bottom two layers between the BL and R layers. This leaves the U and R layers unsolved. The bottom layer center piece can be either solved during this step or left out. It may be advantageous to solve the bottom layer center piece during the stripe. It simplifies the next step to become 2-gen and allows for easier implementation of corner control and other LL reduction strategies, or for ending the first two layers with a one step last slot as described in the "Advanced Last Slot" section above.
3. Solve the remainder of the first two layers. It's not necessary but if following the APB steps exactly, the other half of the BR center is filled in then the five pieces of the last slot are solved. If the bottom layer center was left out during the second step, it can be easily solved during this step.
4. Last layer.

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
        experimental-stickering-mask-orbits="C4RNER:IDIDII,CENTERS:DIIIIII-IDII-IIIIIDDDDD-,EDGES:-IIIII-D--DD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IDIDI-,CENTERS:DI-II--D-D--D-III-DDDDDD,EDGES:D-----DDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:-D-D-D,CENTERS:D-D--D-D-DDDDD----DDDDDD,EDGES:D-D-D-DDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
    ></twisty-player>

</div>

### CFL

Expanding the Nautilus last triple step to solving the three F2L triples makes for a CFOP style method.

1. Centers: Solve the F, BL, and BR large centers. This is sort of like CFOP cross in that it establishes the "E layer" centers and automatically solves the bottom layer edges.
2. F2L: Solve the three triples around the F2L using the Nautilus last triple techniques.
3. Last Layer: Solve the last layer using your preferred way. L6X then L3C, OLL then PLL, or 1LLL.

<div class="applet-grid-nowrap">
    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:IIIII-I-I-----IIII-II-II,EDGES:-I-I-I------"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-I-,CENTERS:-I-IIDIDIDDDDDIIIID--D--,EDGES:DIDIDIDDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:-D-D-D,CENTERS:D-D--D-D-DDDDD----DDDDDD,EDGES:D-D-D-DDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
    ></twisty-player>
</div>

<div class="centered-link-wrapper">
    <a href="https://sites.google.com/view/cfl-fto" class="custom-styled-link" target="_blank" rel="noopener noreferrer">CFL Website</a>
</div>

### EIF FB + Stripe

A completely different approach to F2L is to make EIF the default throughout.

1. FB + Center: Solve a triangle FB on the left and the R layer center. After this step, R r U moves preserve the R layer center. Many 4x4 methods include a step like this, such as Yau, K4, and Meyer.
2. Centers: Solve the L, and B centers, automatically solving the U center. This is a simple step for two reasons. First, there are just three pieces each for the L and B centers. Second, solving the bottom layer triangle between them is mostly R U to attach it to the end of one of these three piece centers.
3. L2T: Solve the last two triples using the same Nautilus techniques. Except there is a little more freedom during the first triple and pseudo slotting or multi slotting can be used.
4. Last Layer

<div class="applet-grid-nowrap">
    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:III-II,CENTERS:IIIII-I-I-I---IIII--IIII,EDGES:-III-I--I-II"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIDII,CENTERS:IIIIID-D-D-DDDIII-DDI--I,EDGES:D---D-DD-DI-"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IDI-,CENTERS:-I-IIDDDDDDDDDIIIDDD-DD-,EDGES:DDDDDDDDDDID"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:-D-D-D,CENTERS:D-D--D-D-DDDDD----DDDDDD,EDGES:D-D-D-DDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>
</div>

### EIF 3x3 Nautilus

Transferring 3x3 Nautilus to an EIF hold still maintains the "r U* r'" F2L property that is the unique property of the Nautilus solving concept. This means that the steps can be FB + R center > 2x2x2 pyramid in the back> F2L minus LS > LS > LL.

<div class="applet-grid-nowrap">
    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:III-II,CENTERS:IIIII-I-I-I---IIII--IIII,EDGES:-III-I--I-II"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IDII,CENTERS:-IIIIDIDIDIDDDIIIIDD--II,EDGES:DIIIDIDDID--"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IDIDII,CENTERS:DIIIIDIDID-DDDIIIIDDDD-I,EDGES:DI-IDIDD-DDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IDIDI-,CENTERS:DI-IIDIDIDDDDDIIIIDDDDD-,EDGES:DIDIDIDDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:-D-D-D,CENTERS:D-D--D-D-DDDDD----DDDDDD,EDGES:D-D-D-DDDDDD"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        camera-longitude="30"
        background="none"
        control-panel="none"
    ></twisty-player>
</div>

## Last Slot Building

When solving the last two centers, the ending will almost always be R U R' or R U' R'. At that point, the three move algorithms used during the triple step can be used to position the corner and a purple triangle ready to be solved using the final R U R' or R U' R'. Once those pieces are in position, perform the initial R move to build the group of last slot pieces. Then solve the bottom triangle and add the pair and center block to the right side layer.

<div class="solve-row">
   <div class="solve-container">

    <twisty-player
        id="fto-player-1"
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-I-,CENTERS:-I-II---------III-------,EDGES:------------"
        experimental-setup-alg="LBLv R U F' U F R'"
        alg="R . // Attach corner to the F layer triangle then use R to build the center
        F' U' F . // Solve the bottom triangle
        U' R' // Solve the pair and half center block"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

    <twisty-alg-viewer id="fto-alg-viewer-1" for="fto-player-1"></twisty-alg-viewer>
  </div>
</div>

If the bottom layer triangle is already solved at the start, or was intentionally solved with the front center's left half, moves such as BR' F' U' F U BR cycle the U layer pieces without affecting the bottom layer triangle. F or BR' can be used to place an unsolved triple at the DR position to allow for free working of other pieces using the three move algorithms.

Community member Fuvash has developed an extension to this technique. The corners can be completely solved in the process, leaving just pure L6X as the last layer step.

<div class="centered-link-wrapper">
    <a href="https://hackmd.io/@fuvash/fto-nautilus-i-lscll" class="custom-styled-link" target="_blank" rel="noopener noreferrer">LSCLL by Fuvash</a>
</div>

## Advanced Last Slot

There isn't a massive number of algorithms for solving the last slot in a single step. At first it may seem to be complicated. But consider that the three pieces of the front half center can only be in a limited number of positions on the upper or front face and the two front triangles can be solved into either position. The corner also has a limited number of positions - it can be in either the upper layer or in its position solved or flipped. The right side triangle can be any of the three right side triangles and one of the right side triangles can always be found within a subset of positions rather than the eight total that exist.

This means that Nautilus could evolve to become a method that reaches F2L-Last Slot then a two step algorithm based finish of Last Slot then Last Layer.

## Corner Control

It may be advantageous to orient the last layer corners during a final step of the F2L. The last triple is a lot of cases, which would increase if adding in LL corner orientation. However, if the bottom triangle can be solved with the centers of Step 2, a ZBLS equivalent could be used. The last F2L corner and the triangle above it can be solved while orienting the LL corners.

Another option would be to combine corner orientation with the advanced last slot described in the previous section. The final moves to solve the advanced LS will typically be R U R' or R U' R'. Setting up to this point first may be a good stepping stone because the LL corners can be easily oriented before or while solving the final insert of R U R' or R U' R'.

## Triangle Control

Another way to reduce cases is to control the triangle permutations. If the triangle locations are modified during the large center building, the last triple cases are reduced. If triangle control is performed during the last triple, it reduces the number of last layer cases and makes last layer recognition even easier.

## Other Ideas

### Last Layer

Outside of 1LLL below are some other interesting ideas:

* Orient the last layer corners then use PLL.
    * There is only one algorithm for orienting the corners, so it will likely be best to combine the corner orientation with solving the last triple of the first two layers. This will then lead directly into PLL. The corners can be easily and intuitively oriented while placing the bottom triple. It may also be viable to combine it with solving the final center of the triple or in a much larger set of one look last triple and corner orientation. Combining corner orientation with the last triple leads to a reduced one look last layer similar to reducing to ZBLL.
* Solve the three corners then the last six triangles.
* Form the three triples on the last layer in any orientation then solve the triples.
* Form four triples at the last triple step then solve the four triples.
* Orient the last layer corners while solving the last six triangles relative to the corners. This forms three triples that can then be permuted using one of two algorithms. This idea was proposed by Vincent Trang.
* Solve one last layer triple in one alg then solve the other two corners and four triangles of the last layer in one alg.

### Last Layer Influencing

* LTCO: Orient the last layer corners while solving the last triple. This is around 600 algorithms.
* LTCPO: Solve the last layer corners while solving the last triple.
* After the step 2 large centers step, solve the last F2L corner and its upper triangle. Then solve the bottom triangle while orienting or solving the last layer corners.
* Orient or solve the last layer corners intuitively during the final moves of the last triple.

### Other

* After step 2 of solving the large centers, solve all triangles then solve the final four corners in a single step.