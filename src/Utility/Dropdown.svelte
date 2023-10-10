<script>
  export let title;
  export let btnImgSrc;
  import { slide } from "svelte/transition";

  let show = false;
  function toggle() {
    show ^= true;
  }
</script>

<div class="showing">
  <button class="btn btn-outline-primary" on:click={toggle}>
    {title}
    <br />
    <br />
    <img class="pic" alt="nunisynth" src={btnImgSrc} />
    <i class="arrow down" />
    <span class="tap">TAP TO EXPAND</span>
  </button>
  {#if show}
    <div class="container" transition:slide>
      <slot>Nothing here yet!</slot>
    </div>
  {/if}
</div>

<style>
  button {
    text-align: left;
    width: 100%;
    margin: auto;
    margin-bottom: 1rem;
    padding: 0.5em 0.25em;
    font-size: 1.75em;
  }
  .arrow {
    float: right;
    border: solid white;
    border-width: 0 5px 5px 0;
    padding: 5px;
    margin: 0.5rem;
  }
  .down {
    transform: rotate(45deg);
    -webkit-transform: rotate(45deg);
  }
  .showing {
    display: sticky;
    top: 0;
  }
  .pic {
    display: block;
    width: 80%;
    height: auto;
    margin: auto;
  }
  .tap {
    height: 2em;
    padding: 0.1em 0.2em;
    animation: flow 1s linear infinite;
    text-align: center;
    /* background: linear-gradient(90deg, white, red, green, blue, purple, orange, cyan, white); */
    background: linear-gradient(
      90deg,
      rgb(68, 68, 68) 0%,
      rgb(255, 213, 0) 20%,
      rgb(68, 68, 68) 35%
    );
    background-size: 300%;
    border-radius: 10px;
    color: white;
    text-shadow: 3px 3px 3px black;
  }
  @keyframes flow {
    0% {
      filter: hue-rotate(0);
    }
    50% {
      filter: hue-rotate(180deg);
    }
    100% {
      filter: hue-rotate(360deg);
    }
  }
</style>
