<article class="clock">
  <div class="hours-container">
    <div class="hours"></div>
  </div>
  <div class="minutes-container">
    <div class="minutes"></div>
  </div>
  <div class="seconds-container">
    <div class="seconds"></div>
  </div>
</article>

<style>
    .clock {
      background: #fff url(/clock.svg) no-repeat center;
      height: 10em;
      position: relative;
      width: 10em;
    }

    .hours {
      background: #000;
      height: 20%;
      left: 48.75%;
      position: absolute;
      top: 30%;
      transform-origin: 50% 100%;
      width: 2.5%;
    }

  .minutes {
    background: #000;
    height: 40%;
    left: 49%;
    position: absolute;
    top: 10%;
    transform-origin: 50% 100%;
    width: 2%;
  }

  .seconds {
    background: red;
    height: 45%;
    left: 49.5%;
    position: absolute;
    top: 14%;
    transform-origin: 50% 80%;
    width: 1%;
  }

  .hours-container {
    position:absolute;
    width:100%;
    height:100%;
    animation: rotate 43200s infinite steps(60);
  }

  .minutes-container {
    position: absolute;
    width:100%;
    height:100%;
    animation: rotate 3600s infinite steps(60);
  }

  .seconds-container {
      width:100%;
      height:100%;
      animation: rotate 60s infinite steps(60);
  }

  @keyframes rotate {
    100% {
      transform: rotateZ(360deg);
    }
  }
</style>