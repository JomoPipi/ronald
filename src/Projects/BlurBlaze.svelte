<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown title="Blur Blaze" btnImgSrc="images/blurblazemainmenu.png">
  <slot>
    <a target="_blank" href="https://blurblaze.vercel.app"> Blur Blaze </a> is
    an straight-line obstacle-dodging time-attack driving game. It works on the
    browser for both mobile and desktop. Try it now or watch a short
    <a target="_blank" href="https://www.youtube.com/watch?v=O2yqg5LwOAI"
      >trailer</a
    >.
    <div>
      <img
        class="fit"
        alt="blurblaze overworld"
        src="images/blurblazeoverworld.png"
      />
      <!-- <img class="fit" alt="blurblaze crash" src="images/blurblazecrash.png" /> -->
      <img class="fit" alt="blurblaze pic 2" src="images/blurblazelevel6.png" />
    </div>
    Made with Three.js, TypeScript, and my own music.
    <br />
    Technical challenges:
    <ul>
      <li>
        <b>Procedural Terrain Generation</b><br /> Terrains are defined as arrays
        of math functions, each representing a different topography. The system combines
        those into single piecewise function that smoothly interpolates between the
        topographies. Chunks are constructed and then, for performance benefit, broken
        into (any (odd) number of) LOD (level of detail) slices, blending the high
        the high-poly center into low-poly outer edges.
      </li>
      <li>
        <b>Object System</b> <br />
        Made a system that efficiently queues up obstacles and activates them on
        collision. Multiple effects can be stacked simultaneously. So you can have
        a lot of fun hitting an ice cube and then sliding hopelessly into an explosive
        barrel.
      </li>
    </ul>

    <img
      class="fit"
      alt="blurblaze overworld"
      src="images/blurblazeoverworld.png"
    />
    <img
      class="fit"
      alt="blurblaze level complete"
      src="images/blurblazelevelcomplete.png"
    />
  </slot>
</Dropdown>

<style>
  .fit {
    display: absolute;
    display: block;
    height: auto;
    margin-bottom: 1em;
    max-width: 75%;
  }
  div {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }
  .strikethrough {
    text-decoration: line-through;
  }
</style>
