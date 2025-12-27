<script>
  export let title;
  export let btnImgSrc;
  import { slide } from "svelte/transition";

  let show = false;
  function toggle() {
    show ^= true;
  }
</script>

<div class="showing" class:open={show}>
  <button class="btn btn-outline-primary" on:click={toggle}>
    <div class="button-title">{title}</div>
    <br />
    <br />
    <img class="pic" alt="nunisynth" src={btnImgSrc} />
    <i class="arrow down" />
    <span class="tap">TAP TO {show ? "COLLAPSE" : "EXPAND"}</span>
  </button>
  {#if show}
    <div class="container" transition:slide>
      <slot>Nothing here yet!</slot>
      <button class="tap tap2" on:click={toggle}
        >TAP TO {show ? "COLLAPSE" : "EXPAND"}
      </button>
    </div>
  {/if}
</div>

<style>
  .container {
    position: absolute;
    top: 100%;
    background-color: white;
    border: 4px solid gray;
    border-top-width: 8px;
    border-bottom-width: 8px;
    z-index: 99;
    padding: 0.5rem 0.5rem 1rem 0.5rem;
  }
  .showing {
    display: sticky;
    position: relative;
    top: 0;
  }
  .showing.open {
    z-index: 10;
  }
  button {
    text-align: left;
    width: 100%;
    margin: auto;
    padding: 0.5em 0.25em;
    font-size: 1.75em;
  }
  .button-title {
    max-height: 0.5em;
    overflow-y: visible;
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
  .pic {
    display: block;
    width: 80%;
    height: auto;
    margin: auto;
    aspect-ratio: 16/10;
    object-fit: contain;
  }
  .tap {
    height: 2em;
    padding: 0.1em 0.2em;
    animation: flow 2s linear infinite;
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
    font-size: 0.75em;
  }
  .tap2 {
    border: 0px;
    width: 50%;
    animation: none;
    margin-top: 0.5rem;
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
