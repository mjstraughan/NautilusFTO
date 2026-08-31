# First Block

The first step is to solve a block consisting of a large center and two triples. Once solved, keep this block on the left side with the U and wide r layers free to turn. A guide for solving the step is provided below, following an introduction to the workings of the FTO so that you can get familiar with its pieces and the way it turns.

<div class="applet-grid-nowrap">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIIIII-IIIIIIII-----I,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv"
        experimental-setup-anchor="end"
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

## Getting to Know the FTO

Before getting started, it is important to know how the FTO works. There are three types of pieces: Corners (four stickers each), Edges (two stickers), and Triangles (one sticker). The pieces called triangles may be considered the center pieces of the FTO, but are typically called triangles in order to distinguish them from steps that involve building large centers of a layer, consisting of three triangles and three edges.

<div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 2rem;">
    <div class="pair-card">
    <div class="applet-grid-nowrap">
        <twisty-player
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:------,CENTERS:IIIIIIIIIIIIIIIIIIIIIIII,EDGES:IIIIIIIIIIII"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            camera-distance="6.2"
            background="none"
            control-panel="none"
        ></twisty-player>
    </div>
    
        <p class="pair-caption">Corners</p>
    </div>

    <div class="pair-card">
    <div class="applet-grid-nowrap">
        <twisty-player
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:IIIIIIIIIIIIIIIIIIIIIIII,EDGES:------------"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            camera-distance="6.2"
            background="none"
            control-panel="none"
        ></twisty-player>
        </div>

        <p class="pair-caption">Edges</p>
    </div>

    <div class="pair-card">
    <div class="applet-grid-nowrap">
        <twisty-player
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:------------------------,EDGES:IIIIIIIIIIII"
            experimental-setup-alg="LBLv"
            experimental-setup-anchor="end"
            camera-distance="6.2"
            background="none"
            control-panel="none"
        ></twisty-player>
        </div>

        <p class="pair-caption">Triangles</p>
    </div>
</div>

When an FTO layer is turned three corners, three edges, and nine triangles are moved (three on the outer face and six around the sides of the layer).

<div class="applet-grid-nowrap">

    <twisty-player
        id="spin-player"
        puzzle="fto"
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

<script>
(function () {
  const player = document.getElementById('spin-player');
  const spinAlg = "U U U U U U U U U";
  const msPerMove = 320;
  const totalMs = spinAlg.trim().split(/\s+/).length * msPerMove;

  customElements.whenDefined('twisty-player').then(() => {
    function loop() {
      player.alg = '';
      requestAnimationFrame(() => {
        player.alg = spinAlg;
        player.play();
      });
    }

    player.alg = spinAlg;
    player.play();
    setInterval(loop, totalMs);
  });
})();
</script>

A final important note is to check the Notation page to learn the labels for each layer so that you can follow along with algorithms. The Notation page provides the notation for when holding the FTO with a corner in the front, an edge in front hold, and also covers rotations of the entire FTO.

## Center

The simplest way to build the first block is to start by solving a large center. This center consists of three inner centers (triangles) and three edges. This center should be kept on the BL layer. For visibility the applets will show the center building process with the center on the front.

<div class="applet-grid-nowrap">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:IIIIIIIII-IIIIIIII-II-II,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv Uv'"
        camera-latitude="-15"
        camera-longitude="0"
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

To start solving the center, build a half center. There are four different half centers that you can start with. Build the one that is easiest or that you see first. Take care to solve the edges in the correct order for the color scheme. If you are unsure after scrambling, check the corners to know. If you are using the same color scheme as on this site, follow the applets and solve the same pieces. To build a half center, start by choosing an edge. Any edge is ok. Then find a triangle and pair it with the edge. The triangle can usually be attached to the edge using just a couple of moves. In the example below, the left side is turned to bring down a triangle on the upper layer to match with an edge, then a second edge is attached to form a half center.

<div class="solve-row">
    <div class="solve-container">

        <twisty-player
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:IIIIIIIIIIIIIIIIIIIII-II,EDGES:IIIIIIIIII--"
            experimental-setup-alg="LBLv Uv' u' R' U' L'"
            alg="L U R u"
            background="none"
            camera-latitude="-15"
            camera-longitude="0"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

    </div>
</div>

Next, build the other half center that consists of an edge and two triangles. Locate the final edge that belongs with the center then attach a triangle to either side, then attach the new half center to form the complete large center.

<div class="solve-container">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:IIIIII,CENTERS:IIIIIIIII-IIIIIIII-II-II,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv Uv' R U R' U R'"
        alg="R U' R U' R'"
        background="none"
        camera-latitude="30"
        camera-longitude="0"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

</div>

## First Triple

Once the center is complete, the two triples will be solved. A triple is a corner and two triangles.

<div class="solve-container">

    <twisty-player
    puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIIIIIDIIIIIIIID--D-I,EDGES:IIIIIIIDIIDD"
        experimental-setup-alg="LBLv Uv'"
        camera-latitude="-15"
        camera-longitude="0"
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 320px;"
    ></twisty-player>

</div>

From this point forward, the large center will be kept on the BL layer in the applets.

Keeping the solved center on the back left layer, solve the first triple. Find one of the corners and attach the two triangles that match the colors of the large center. In this example, the back triple will first be solved. In the following applet, the corner is on the upper layer in the front and the white triangle is on the back layer. The two pieces can be paired with a turn of the right side layer. The green triangle can then be moved to the upper layer using a turn of the front layer, then attached to the corner and triangle pair by turning the U layer and temporarily moving the pair below the upper layer. Once formed, the triple is oriented such that the corner has the first step center color facing upwards, so the triple is moved to the upper back right position then solved by turning the back right (BR) layer. If the triple had been oriented with the other color facing upwards, the sequence to place would have been F BR'.

<div class="solve-container">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIII-IIIIIIII-I--II,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv BR' U R' U R U' F R'"
        alg="R . // Attach first triangle
        F' U R' U' R . // Attach second triangle
        U' BR // Attach triple to the center"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

</div>

## Second Triple

Solving the second triple uses the same process. First, pair the corner with a triangle. In the following applet, the corner starts out on the upper layer in the front. There is a triangle on the back layer. A single turn of the right side layer pairs the two pieces. The second triangle is on the bottom layer. A turn of the upper layer moves the corner and triangle into position for a slice turn that attaches the second triangle to form a triple. The triple is oriented such that the original large center color is facing upwards, so turning the front layer correctly places the triple. If the triple had been oriented the other way, the sequence r' F would have solved it.

<div class="solve-container">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-II,CENTERS:-IIIIIIII-IIIIIIII-----I,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv F 2R' U' R'"
        alg="R . // Attach first triangle
        U 2R . // Attach second triangle
        F' // Attach triple to the center"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

</div>

## Arrow Block

Once comfortable with solving the first block using the three steps of center and two triples, the steps can be combined. A triple can be combined with the center in a single step to form an arrow block. Two important strategies will be shown through examples.

<div class="solve-container">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIII-IIIIIIII-I--II,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv Uv' Rv Uv'"
        alg=""
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

### Strategy 1: Small Arrow Block

Using this strategy, a smaller arrow block is built then the remainder of the center is completed. The benefit of starting with a smaller arrow block is that it takes care of the two additional outside triangle pieces that need to be attached to the corner. If the large center is built first, as in the basic three step strategy, movement is restricted and there is an increase to the number of moves needed to build and add the corner and two triangles.

<div class="solve-container">

    <twisty-player
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIIIIIIIIIIIIII--II,EDGES:IIIIIIIIII--"
        experimental-setup-alg="LBLv Uv' Rv Uv'"
        alg=""
        background="none"
        control-panel="none"
        style="max-width: 300px; height: 300px;"
    ></twisty-player>

</div>

#### Examples

<div class="solve-row">

    <div class="solve-container">

        <twisty-player
            id="fto-player-1"
            puzzle="fto"
            experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIIIIIIIIIIIIII--II,EDGES:IIIIIIIIII--"
            experimental-setup-alg="LBLv Uv' Rv Uv' F D' BL' R B"
            alg="B' R' . // Build half center
            BL D F' // Build and add triple"
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
            experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIIIIIIIIIIIIII--II,EDGES:IIIIIIIIII--"
            experimental-setup-alg="LBLv Uv' Rv Uv' br' BL' R' D' F'"
            alg="F . // Edge plus triangle
            D R . // Corner plus triangle
            BL br // Edge plus triangle"
            background="none"
            style="max-width: 300px; height: 400px; margin-top: -30px;"
        ></twisty-player>

        <twisty-alg-viewer
            for="fto-player-2"
        ></twisty-alg-viewer>

    </div>
</div>

After the completion of the small arrow block, add the three remaining pieces of the large center to complete the large arrow block.

### Strategy 2: Half Center First

Another useful strategy is to start by building a half center. Then build and add the remaining pieces to from the arrow block. This strategy is more restrictive than the small arrow block strategy, due to solving the initial half center at the start versus leaving it for the end in the small arrow block strategy. However, this strategy is still useful because the left or right half center of the arrow block may already be solved, or be easy to solve in many scrambles.

#### Examples

<div class="solve-row">

  <div class="solve-container">
    <twisty-player
        id="fto-player-3"
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIII-IIIIIIII-I--II,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv Uv' Rv Uv' R' D' BL' R' D' F U R"
        alg="R' U' F' . // Half center plus triangle
        D R . // Edge and two triangles
        BL D R // Corner and last triangle"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-3"></twisty-alg-viewer>
  </div>

  <div class="solve-container">
    <twisty-player
        id="fto-player-4"
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-IIII,CENTERS:-IIIIIIII-IIIIIIII-I--II,EDGES:IIIIIII-II--"
        experimental-setup-alg="LBLv Uv' Rv Uv' R' F BL' D BR D'"
        alg="// Half center built
        D BR' D' BL F' R // Build remainder of the block"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

    <twisty-alg-viewer for="fto-player-4"></twisty-alg-viewer>
  </div>

</div>