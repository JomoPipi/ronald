<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown title="BLOOD BLAZE" btnImgSrc="images/bloodblaze.png">
  <slot>
    <a target="_blank" href="https://bloodblaze.io"> BLOOD BLAZE</a> is a 2D
    top-down fast-paced multiplayer shooter game. It works on mobile and desktop
    browsers. Shoot your friends in the face and enjoy.
    <div>
      <img class="fit" alt="bloodblaze pic" src="images/bloodblaze3.png" />
      <img class="fit" alt="bloodblaze pic 2" src="images/bloodblaze2.png" />
    </div>
    It also is now in 3D:
    <img class="fit" alt="bloodblaze pic 2" src="images/bloodblaze4.png" />
    <span class="strikethrough"
      >Go play, right now!
      <a target="_blank" href="https://bloodblaze.io">
        https://bloodblaze.io
      </a></span
    >

    Domain name expired. One day it will be back though!
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
