
  <div class="circle">
    <div class="square big" />
    <div class="square small" />
  </div>

<style>
  body {
    background: #293462;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .circle {
    height: 200px;
    width: 200px;
    border-radius: 50%;
    background: #FFF1C1;
    position: relative;
    overflow: hidden;
  }

  .square {
    background: #FE5F55;
    transform: rotate (45deg);
    position: absolute;
  }

  .big {
    height: 150px;
    width: 150px;
    left: 66px;
    top: 90px;
  }
  .small {
    height: 69px;
    width: 69px;
    left: -5px;
    top: 143px;
  }
</style>
