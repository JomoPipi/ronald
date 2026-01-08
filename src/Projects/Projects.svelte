<script>
  import NUNISYNTH from "./NUNISYNTH.svelte";
  import LambdaCalcEval from "./LambdaCalcEval.svelte";
  import WiFiCar from "./WiFiCar.svelte";
  import CodingPro from "./CodingPro.svelte";
  import Bloodblaze from "./BLOODBLAZE.svelte";
  import MotorProject from "./MotorProject.svelte";
  import CryptoPumpNotifier from "./CryptoPumpNotifier.svelte";
  import BlurBlaze from "./BlurBlaze.svelte";
  import RWS from "./RWS.svelte";
</script>

<div class="grid">
  <div class="item"><RWS /></div>
  <div class="item"><NUNISYNTH /></div>
  <div class="item"><BlurBlaze /></div>
  <div class="item"><CryptoPumpNotifier /></div>
  <div class="item"><Bloodblaze /></div>
  <div class="item"><LambdaCalcEval /></div>
  <div class="item"><CodingPro /></div>
  <div class="item"><WiFiCar /></div>
  <div class="item"><MotorProject /></div>
</div>

<style>
  .grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    left: 0;
  }
  div > .item:nth-child(even) {
    transform: translateY(50%);
  }
  /* Force earlier items to sit ON TOP of later items */
  /* very brute-force-ish, but... whatever  */
  /* prettier-ignore */
  div > .item:nth-child(1) { z-index: 10; } /* prettier-ignore */
  div > .item:nth-child(2) { z-index: 9; } /* prettier-ignore */
  div > .item:nth-child(3) { z-index: 8; } /* prettier-ignore */
  div > .item:nth-child(4) { z-index: 7; } /* prettier-ignore */
  div > .item:nth-child(5) { z-index: 6; } /* prettier-ignore */
  div > .item:nth-child(6) { z-index: 5; } /* prettier-ignore */
  div > .item:nth-child(7) { z-index: 4; } /* prettier-ignore */
  div > .item:nth-child(8) { z-index: 3; }

  @media screen and (max-width: 768px) {
    .grid {
      grid-template-columns: 1fr;
    }
    div > .item:nth-child(even) {
      transform: none;
    }
  }
</style>
