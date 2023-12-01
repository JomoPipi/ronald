<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown title="Asynchronous Reluctance Motor" btnImgSrc="images/motorpic.png">
  <slot>
    To make this work, I learned how to use electromagnets, hall effect sensors,
    and arduino interrupts.
    <br />

    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/E56WVJSrQc0?si=YY_gKwnTsBt4oCCO&amp;start=22"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
      allowfullscreen
    />
  </slot>
</Dropdown>

<style>
  iframe {
    display: block;
    max-width: 100%;
    height: auto;
    margin: auto;
    margin-top: 10px;
  }
</style>
