<div class="solve-row">
   <div class="solve-container">

    <twisty-player
        id="fto-player-1"
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-I-,CENTERS:-I-II---------III------I,EDGES:------------"
        experimental-setup-alg="LBLv R U' BR U BR' R'"
        alg="R . // Attach corner to the triangle
BR U' BR' . // Attach the corner and triangle pair to the half center
U R' // Solve the pair and half center group"
        camera-longitude="60"
        background="none"
        style="max-width: 300px; height: 400px; margin-top: -30px;"
    ></twisty-player>

    <twisty-alg-viewer id="fto-alg-viewer-1" for="fto-player-1"></twisty-alg-viewer>
  </div>
</div>

If the corner is already paired with a correct triangle before starting, solve the pair in the F2L using one of the separation moves.

<div class="solve-row">
  <div class="solve-container">

    <twisty-player
        id="fto-player-2"
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-I-,CENTERS:-I-II---------III------I,EDGES:------------"
        experimental-setup-alg="LBLv BR U BR'"
        alg="BR U' BR' . // Solve preformed pair with triangle to the right of the corner"
        camera-longitude="60"
        background="none"
        style="max-width: 300px; height: 500px;"
    ></twisty-player>

    <twisty-alg-viewer id="fto-alg-viewer-2" for="fto-player-2"></twisty-alg-viewer>
  </div>

  <div class="solve-container">

    <twisty-player
        id="fto-player-3"
        puzzle="fto"
        experimental-stickering-mask-orbits="C4RNER:I-I-I-,CENTERS:-I-II---------III------I,EDGES:------------"
        experimental-setup-alg="LBLv F' U' F"
        alg="F' U F . // Solve preformed pair with triangle to the left of the corner"
        camera-longitude="60"
        background="none"
        style="max-width: 300px; height: 500px;"
    ></twisty-player>

    <twisty-alg-viewer id="fto-alg-viewer-3" for="fto-player-3"></twisty-alg-viewer>
  </div>
</div>

<script>
function setupAlgRelabel(viewerId, displayMoves) {
  const viewer = document.getElementById(viewerId);
  if (!viewer) return;

  function relabel() {
    const moveEls = viewer.querySelectorAll('.twisty-alg-move');
    if (moveEls.length !== displayMoves.length) return false;

    let successCount = 0;
    moveEls.forEach((el, i) => {
      // Look into the element or its shadow root for text nodes
      const textEl = el.shadowRoot 
        ? el.shadowRoot.querySelector('a, span') 
        : el.querySelector('a, span');

      if (textEl && textEl.textContent !== displayMoves[i]) {
        textEl.textContent = displayMoves[i];
        successCount++;
      } else if (textEl) {
        successCount++;
      }
    });

    // Only disconnect when ALL moves have been successfully targeted and updated
    return successCount === displayMoves.length;
  }

  const observer = new MutationObserver(() => {
    if (relabel()) observer.disconnect();
  });

  observer.observe(viewer, { childList: true, subtree: true });
  
  // Initial check in case it's already rendered
  if (relabel()) observer.disconnect();
}

// Ensure execution runs after DOM ready (helps with MkDocs SPA navigation)
document.addEventListener("DOMContentLoaded", () => {
  setupAlgRelabel('fto-alg-viewer-1', ["F", "R", "U'", "R'", "U", "F'"]);
  setupAlgRelabel('fto-alg-viewer-2', ["R", "U'", "R'"]);
  setupAlgRelabel('fto-alg-viewer-3', ["L'", "U", "L"]);
});
</script>