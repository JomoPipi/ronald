<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown title="NUNISYNTH" btnImgSrc="images/nunisynth.png"
  ><slot>
    <a target="_blank" href="https://noodlesynth.com"> NUNISYNTH</a> is a
    <a
      target="_blank"
      href="https://en.wikipedia.org/wiki/Graph_(discrete_mathematics)"
      >graphical</a
    >
    modular audio synthesizer based on the
    <a
      target="_blank"
      href="https://developer.mozilla.org/en-US/docs/Web/API/Web_Audio_API"
      >Web Audio API</a
    >. Its original purpose was to facilitate exploring and experimenting with
    the API, but it evolved into something more.
    <!-- <img class="nunisynth-pic-0 fit" alt="nunisynth" src="https://nunisynth.com/static/media/allnodes.90720be2.png"> -->

    <ul>
      <li>
        It's been through several iterations of UI refinements. Even though it
        gives you fine-grained audio control, it lets users create intricate
        things with relatively few steps.
      </li>
      <li>
        Auxiliary utilities (for example: scale builders, sample-generating
        formulas, visualizers, keyboarding, recording, importing, exporting,
        keyboard shortcuts, saving, loading, and more) were added.
      </li>
      <li>
        A number of custom Web Audio nodes were added, including Automation,
        Sample Sequencer, Gate Sequencer, Sample Piano Roll, Mono Piano Roll,
        Recorder, Module.
      </li>
      <li>
        Modules play a big role. They are basically nested graphs. Users can
        save their own custom modules and reuse them in any project. A handful
        of helpful modules are provided by default.
      </li>
      <li>
        An earlier version of the product was released and sold on
        <a
          target="_blank"
          href="https://nunisynth.gumroad.com/l/gwIwi?layout=profile"
        >
          Gumroad</a
        >.
      </li>
    </ul>
    <div>
      <iframe
        width="560"
        height="315"
        src="https://www.youtube.com/embed/M2EJSqIGXRY"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>
  </slot></Dropdown
>

<style>
  li {
    margin: 0.5em 0em;
  }
  iframe {
    display: block;
    max-width: 100%;
    height: auto;
    margin: auto;
    margin-top: 10px;
  }
</style>
