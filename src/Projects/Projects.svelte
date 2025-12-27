<script>
  import NUNISYNTH from "./NUNISYNTH.svelte";
  import LambdaCalcEval from "./LambdaCalcEval.svelte";
  import WiFiCar from "./WiFiCar.svelte";
  import CodingPro from "./CodingPro.svelte";
  import Bloodblaze from "./BLOODBLAZE.svelte";
  import MotorProject from "./MotorProject.svelte";
  import CryptoPumpNotifier from "./CryptoPumpNotifier.svelte";
  import BlurBlaze from "./BlurBlaze.svelte";
</script>

<div class="grid">
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
  div > :nth-child(even) {
    transform: translateY(50%);
  }
  @media screen and (max-width: 768px) {
    .grid {
      grid-template-columns: 1fr;
    }
  }
</style>
