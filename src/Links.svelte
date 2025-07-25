<div class="links-container">
  <div class="links-list">
    <div class="email">Ronaldmcorona@gmail.com</div>
    <hr />
    <div>
      <a target="_blank" href="https://github.com/Jomopipi"
        >github.com/Jomopipi</a
      >
    </div>
    <hr />
    <div>
      <a target="_blank" href="./images/condensed.pdf">Resume</a>
    </div>
  </div>

  <img src="./images/ollie.png" alt="ollie" />
</div>

<style>
  .links-container {
    display: flex;
    gap: 2em;
    align-items: center;
    justify-content: center;
  }
  .email {
    text-decoration: dotted underline;
  }
  img {
    width: 40%;
    box-shadow: 0px 0px 8px black;
    border-radius: 1em;
  }
  .links-list {
    list-style: square;
    text-transform: uppercase;
  }

  @media (max-width: 768px) {
    div {
      flex-direction: column;
    }
    img {
      width: 70%;
      border-radius: 0.5em;
    }
  }
</style>
