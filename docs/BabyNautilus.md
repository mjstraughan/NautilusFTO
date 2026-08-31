# Baby Nautilus

This is an adaption of Nautilus to Baby FTO (aka Skewb Diamond, aka 2x2 FTO). It is best to directly solve the first layer in the best way for each scramble, then finish with CLL. But this set of steps is a way to simplify the first layer as a way to get to the point of being able to handle full layer building. These steps align with Nautilus on FTO because the centers in the R layer in Baby Nautilus can be viewed as the large centers of the wide r layers in FTO Nautilus. This method follows the same steps of FB > Centers > Triple > Last Layer.

<div class="centered-link-wrapper">
    <a href="https://docs.google.com/spreadsheets/d/1hyGv6J2Xy1CHW__pmOk2DNyC7_VQ8FGuOAAVjwwXmTg/edit?usp=sharing" class="custom-styled-link">Baby FTO Algorithm List</a>
</div>

<div class="applet-grid-nowrap">

    <twisty-player
        puzzle="baby_fto"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

## First Block

Solve two corners and the two centers between them, then keep the block at the bottom left.

<div class="solve-row">

    <div class="solve-container">

        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-IIII-,CENTERS:IIIII-I-"
            experimental-setup-alg="LBLv"
            camera-latitude="-15"
            camera-longitude="-120"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>

    </div>

    <div class="solve-container">

        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-IIII-,CENTERS:IIIII-I-"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>

    </div>
</div>

## Triple

Finish the first layer by solving the last two centers and the last corner. This can be simplified to turning the R layer to move the U center to the U layer, automatically aligning all R layer surrounding centers. Then solve the last corner of the first layer. The corner substep aligns with FTO Nautilus because there are no small center triangles on Baby FTO, leaving just a corner to be solved.

<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 2rem;">
    <div class="pair-card">
    <div class="applet-grid-nowrap">
        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-IIII-,CENTERS:III-----"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>
    </div>
    
    <p class="pair-caption">1: Turn the R layer to align the centers.</p>
    </div>

    <div class="pair-card">
    <div class="applet-grid-nowrap">
        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>
        </div>

        <p class="pair-caption">2: Solve the last corner of the first layer.</p>
    </div>
</div>

There are just three cases for solving the final corner.

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-1"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R U R'"
        alg="R U' R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-1"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-2"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R U' R'"
        alg="R U R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-2"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-3"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R' U' R' U' R'"
        alg="R U R U R"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-3"></twisty-alg-viewer>
  </div>

</div>

The centers and the final corner can be combined into a single step of solving the triple on the first layer. Below are the solutions for this combined step. You already know the three cases above when the centers are aligned, leaving just eight additional cases to learn. Really this step is intuitive because you simply align a center with the corner then attach that pair to the other center.

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-4"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R'"
        alg="R"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-4"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-5"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R"
        alg="R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-5"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-6"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R U R"
        alg="R' U' R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-6"></twisty-alg-viewer>
  </div>

</div>

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-7"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R' U' R'"
        alg="R U R"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-7"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-8"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R U' R"
        alg="R' U R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-8"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-9"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R U R' U' R'"
        alg="R U R U' R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-9"></twisty-alg-viewer>
  </div>

</div>

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-10"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R' U R'"
        alg="R U' R"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-10"></twisty-alg-viewer>
  </div>

    <div class="solve-container">
    <twisty-player
        id="fto-player-11"
        puzzle="baby_fto"
        experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-----"
        experimental-setup-alg="LBLv R U R U' R'"
        alg="R U R' U' R'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-11"></twisty-alg-viewer>
  </div>
</div>

## CLL

Now solve the corners of the last layer using a single algorithm. There are only five algorithms to learn.

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-12"
        puzzle="baby_fto"
        experimental-setup-alg="LBLv U BL U' BL U BL U' BL"
        alg="BL' U BL' U' BL' U BL' U'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-12"></twisty-alg-viewer>
    <p class="pair-caption">{BL, L} U' R U' R' U' R U' R'</p>
  </div>

    <div class="solve-container">
    <twisty-player
        id="fto-player-13"
        puzzle="baby_fto"
        experimental-setup-alg="LBLv BL' U BL' U' BL' U BL' U'"
        alg="U BL U' BL U BL U' BL"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-13"></twisty-alg-viewer>
    <p class="pair-caption">{BL, L} R U R' U R U R' U</p>
  </div>
</div>

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-14"
        puzzle="baby_fto"
        experimental-setup-alg="LBLv L R' L' R U R' L R L' U'"
        alg="(U) L R' L' R U' R' L R L'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-14"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-15"
        puzzle="baby_fto"
        experimental-setup-alg="LBLv R' L R L' R' L R L' U'"
        alg="U L R' L' R L R' L' R"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-15"></twisty-alg-viewer>
    <p class="pair-caption">(U) {L, F} U R' U' R U R' U' R</p>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-16"
        puzzle="baby_fto"
        experimental-setup-alg="LBLv L R' L' R L R' L' R U"
        alg="(U') R' L R L' R' L R L'"
        background="none"
        style="max-width: 300px; height: 425px; margin-top: -50px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-16"></twisty-alg-viewer>
    <p class="pair-caption">(U') {L, F} R' U R U' R' U R U'</p>
  </div>

</div>

## One Step First Layer

The most advanced form of solving the first layer is to solve it in the way that best fits the current scramble.

<div class="solve-row">

    <div class="solve-container">

        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-I---"
            experimental-setup-alg="LBLv"
            camera-latitude="-15"
            camera-longitude="0"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>

    </div>

    <div class="solve-container">

        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-I---"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>

    </div>
</div>

Another idea to advance first layer solving is to leave out the D center when building the first block, then solve the remainder of the first layer. This is the DR corner and D, F, and BR centers at 35 cases.

<div class="solve-row">

    <div class="solve-container">

        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-IIII-,CENTERS:IIIII-II"
            experimental-setup-alg="LBLv"
            camera-latitude="-15"
            camera-longitude="0"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>

    </div>

    <div class="solve-container">

        <twisty-player
            puzzle="baby_fto"
            experimental-stickering-mask-orbits="C4RNER:-I-II-,CENTERS:III-I---"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            background="none"
            control-panel="none"
            style="max-width: 300px; height: 350px;"
        ></twisty-player>

    </div>
</div>

## Advancements

To really advance the method, part of solving the first layer can be combined with solving the last layer. Some ideas below:

* First layer minus one corner then solve the last corner and last layer in one step.
* First Block then solve the remaining pieces within the U and R layers. This is 11 cases if Corner Permutation First Block is performed and 107 cases with normal First Block.
* First Block minus the D center then solve the remaining pieces in 395 cases.

## Alternate Steps

Below is another set of steps that could also be viewed as a Nautilus adaption. This one views the D center as the bottom triangle of the last F2L triple in FTO Nautilus. These steps are a simplified version of the advanced first layer idea above.

* FB: Pair two adjacent corners on the first layer and the triangle that belongs between them.
* Centers: Simply turn R to move the yellow center to the upper layer.
* Pair: Solve the final two pieces of the first layer.
* CLL: Solve the last layer.