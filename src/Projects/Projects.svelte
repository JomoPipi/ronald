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

<div>
  <NUNISYNTH />
  <BlurBlaze />
  <CryptoPumpNotifier />
  <Bloodblaze />
  <LambdaCalcEval />
  <CodingPro />
  <WiFiCar />
  <MotorProject />
</div>

<style>
  div {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    left: 0;
  }
  @media screen and (max-width: 768px) {
    div {
      grid-template-columns: 1fr;
    }
  }
</style>
