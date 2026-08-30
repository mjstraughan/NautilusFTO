# Last Layer

In the final step, solve the last layer. The major advantage of ending in a last layer is that recognition is easy. All of the necessary stickers are on the sides of the last layer, with two out of three sides in view. During the previous step of solving the last triple look ahead to watch a single triangle go to the back layer and recognition will be completely two sided.

<div class="applet-grid-nowrap">
<twisty-player
    puzzle="fto"
    experimental-stickering-mask-orbits="C4RNER:-D-D-D,CENTERS:D-D--DDDDDDDDD---DDDDDDD,EDGES:DDDDDDDDDDDD"
experimental-setup-alg="LBLv"
experimental-setup-anchor="end"
    background="none"
control-panel="none"
    style="max-width: 300px; height: 300px;"
  ></twisty-player>
</div>

## Part 1: Last Six Triangles (L6X)

### Beginner

The first step to solving the last layer is to solve the last six triangles. In the basic version, this step is accomplished in 2 sub steps. First, one side is completed using an algorithm then the other two sides are solved using the same set of algorithms. First, check for a triangle and edge pair. This is called a diamond. Move the other triangle to the diamond to complete a side.

If there are no diamonds, use one of the algorithms to move a triangle to an edge and form a diamond. Then follow the process of completing a side. Once one side is completed, use the same algorithms to solve the remaining two sides. It only takes one application of an algorithm to solve both sides at once.

The applets depict an overhead view of the last layer with the front corner at the bottom.

<div class="pair-card">
  <div class="applet-grid-nowrap">
    <twisty-player
      puzzle="fto"
      experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
      experimental-setup-alg="LBLv U'"
      alg="U' F' r U R' U' r' F R"
      experimental-setup-anchor="end"
      camera-latitude-limit="180"
      camera-latitude="90"
      camera-distance="6.2"
      background="none"
      control-panel="none"
    ></twisty-player>

    <twisty-player
      puzzle="fto"
      experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
      experimental-setup-alg="LBLv U"
      alg="U' F' r U R' U' r' F R"
      experimental-setup-anchor="end"
      camera-latitude-limit="180"
      camera-latitude="90"
      camera-distance="6.2"
      background="none"
      control-panel="none"
    ></twisty-player>
  </div>
  
  <p class="pair-caption">{U, R} (U') R U R' U' R' r U R U' r'</p>
</div>

<div class="pair-card">
  <div class="applet-grid-nowrap">
    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
        experimental-setup-alg="LBLv"
        alg="T' F' R' L' R L r' R L' R' L r F T"
        experimental-setup-anchor="end"
        camera-latitude-limit="180"
        camera-latitude="90"
        camera-distance="6.2"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
        experimental-setup-alg="LBLv U'"
        alg="T' F' R' L' R L r' R L' R' L r F T"
        experimental-setup-anchor="end"
        camera-latitude-limit="180"
        camera-latitude="90"
        camera-distance="6.2"
        background="none"
        control-panel="none"
    ></twisty-player>
    </div>

    <p class="pair-caption">{U, R} F' U R U' r' L R' L' r F</p>
</div>

<div class="pair-card">
  <div class="applet-grid-nowrap">
    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
        experimental-setup-alg="LBLv U'"
        alg="U' R' F' r U R U' r' F"
        experimental-setup-anchor="end"
        camera-latitude-limit="180"
        camera-latitude="90"
        camera-distance="6.2"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
        experimental-setup-alg="LBLv U"
        alg="U' R' F' r U R U' r' F"
        experimental-setup-anchor="end"
        camera-latitude-limit="180"
        camera-latitude="90"
        camera-distance="6.2"
        background="none"
        control-panel="none"
    ></twisty-player>
    </div>

    <p class="pair-caption">{U, R} (U) r U R' U' r' L R L'</p>
</div>

<div class="pair-card">
  <div class="applet-grid-nowrap">
    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
        experimental-setup-alg="LBLv U"
        alg="U r' F' r U R' r U' r' F R"
        experimental-setup-anchor="end"
        camera-latitude-limit="180"
        camera-latitude="90"
        camera-distance="6.2"
        background="none"
        control-panel="none"
    ></twisty-player>

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:III-II-I-IIIIIII--IIIIII,EDGES:I-I-I-IIIIII"
        experimental-setup-alg="LBLv"
        alg="U r' F' r U R' r U' r' F R"
        experimental-setup-anchor="end"
        camera-latitude-limit="180"
        camera-latitude="90"
        camera-distance="6.2"
        background="none"
        control-panel="none"
    ></twisty-player>
    </div>

    <p class="pair-caption">{U,R} (U) L R' L' r U R U' r'</p>
</div>