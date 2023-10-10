<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown
  title="NodeMCU Car"
  btnImgSrc="https://raw.githubusercontent.com/JomoPipi/nodemcu-wifi-car/master/IMG_1726.jpg"
>
  <slot>
    I learned
    <ul>
      <li>
        <a target="_blank" href="https://www.youtube.com/watch?v=nzkbhGDTL5w">
          how to build chassis</a
        >,
      </li>
      <li>
        <a target="_blank" href="https://www.youtube.com/watch?v=d7oFD-zQpuQ">
          how to control DC motors</a
        >, <br />
      </li>
      <li>
        <a
          target="_blank"
          href="https://www.instructables.com/id/Esp8266Websockets-RGB-LED-controller/"
          >how Websocket Nodemcu connections work</a
        >,
      </li>
    </ul>
    and I pieced this information together to learn to create inexpensive remote
    control cars that you can control from your phone.
    <br />

    <iframe
      width="560"
      height="315"
      src="https://www.youtube.com/embed/6uOXedOu_T4?&t=45"
      title="YouTube video player"
      frameborder="0"
      allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
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
