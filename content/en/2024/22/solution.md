---
title: Day 22 - Solution
toc: false
type: docs
---


Given the kings' position, whoever can castle must be Black.

Assume Red is White (thus Blue can castle). The last move by Blue (a.k.a. Black) must have been h7-h6, but what was the move before that? It must have been with a piece that is no longer on the board. It cannot have been with the blue knight that was captured on b3 as Red needs 2 retractions (plus the check retraction) before that knight can appear on the board. Therefore, the second last move by Black must have been with the missing rook and the last moves must have been (in reverse order): Ng8-f6+, h7-h6, Nh6xRg8, Rh8-g8. However, the fact that the missing rook was captured on g8 means the position has "the wrong parity". Indeed, it can be shown that both players made an even number of moves to reach the diagram position, so it should be Red to move (since Red started the game), but Blue is in check!

We conclude Red cannot be White, thus Blue must be White. It is not hard to see that the position has no legality issues in that case.




<!--
<br>
<br>
<iframe 
    style="width: 100%; height: 80vh;" 
    src="https://lichess.org/study/embed/PrONOirR/uj3Wrzet" 
    frameborder="0">
</iframe> 
-->