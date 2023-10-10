<script>
  export let name;
  import Summary from "./Summary.svelte";
  import Projects from "./Projects/Projects.svelte";
</script>

<main>
  <div id="pages">
    <div class="title-pic">
      <img class="ronald-img" alt="ronald" src="images/ronald.jpg" />
      <div class="flex-vert">
        <h1>{name} Corona</h1>
        <h4>writes interactive applications</h4>
      </div>
    </div>
    <!-- <div id="main__grid"></div> -->
    Ronaldmcorona@gmail.com
    <br />
    <a target="_blank" href="https://github.com/JomoPipi"
      >https://github.com/JomoPipi</a
    >

    <Summary />
    <div id="main-content">
      <br /><br />

      <Projects />

      <br /><br />

      Ronaldmcorona@gmail.com
      <br />
      <a target="_blank" href="https://github.com/JomoPipi"
        >https://github.com/JomoPipi</a
      >
    </div>
  </div>
</main>

<style>
  main {
    display: flex;
    align-items: center;
    justify-content: center;
  }
  #main-content {
    padding: 2% 10%;
    width: 1200px;
    max-width: 95vw;
  }

  .ronald-img {
    width: 40%;
    margin: 5%;
    border-radius: 40px;
    box-shadow: 8px 8px 8px black;
  }

  .title-pic {
    display: -webkit-box;
    display: -ms-flexbox;
    display: flex;
    -ms-flex-pack: distribute;
    justify-content: space-around;
    -webkit-box-align: center;
    -ms-flex-align: center;
    align-items: center;
    padding: 4%;
  }

  /*# sourceMappingURL=styles.css.map */
</style>
