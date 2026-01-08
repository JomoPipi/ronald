<script>
  import Dropdown from "../Utility/Dropdown.svelte";
</script>

<Dropdown title="RWS Console" btnImgSrc="images/rws-1.png">
  <slot>
    <a target="_blank" href="https://rws-console.vercel.app"> RWS Console</a> Is
    a container-as-a-service platform that runs on Kubernetes and is powered by
    a beat-up laptop I found on the street. You can create a free account,
    launch a service, receive a link to your deployment, and watch the logs -
    for free.
    <div>
      <img class="fit" alt="bloodblaze pic" src="images/rws-2.png" />
    </div>
    Try it out right now
    <a target="_blank" href="https://rws-console.vercel.app">
      https://rws-console.vercel.app
    </a>.
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
</style>
