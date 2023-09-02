<main>
  <div class="angry-grid">
    <div id="item-0">3 × 2(color:blue-400)</div>
    <div id="item-1">2 × 2(color:teal-400)</div>
    <div id="item-2">5 × 4(color:rose-100)</div>
    <div id="item-3">2 × 6(color:blue-400)</div>
    <div id="item-4">1 × 6(color:fuchsia-400)</div>
    <div id="item-5">
      4 × 4(color:yellow-400)
      <!-- <section id="squareOnTop">
        <div class="circle">
          <div class="square big" />
          <div class="square small" />
        </div>
      </section> -->
    </div>
    <div id="item-6">4 × 2(color:emerald-400)</div>
  </div>
</main>

<style>
  :root {
    --main-radius: 5px;
    --main-padding: 5px;
  }

  .angry-grid {
    display: grid;
    font-size: 12px;
    font-weight: 800;
    color: #004d40;
    grid-template-rows: 1fr 1fr 1fr 1fr;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr;

    text-align: center;
    height: 100vh;
  }

  #item-0 {
    background-color: #42a5f5;
    grid-row-start: 1;
    grid-column-start: 1;
    color: black;
    line-height: 230px;
    text-align: center;
    vertical-align: central;
    grid-row-end: 3;
    grid-column-end: 2;
  }
  #item-1 {
    background-color: #26a69a;
    grid-row-start: 3;
    grid-column-start: 1;
    color: black;
    line-height: 150px;
    text-align: center;
    vertical-align: central;
    grid-row-end: 4;
    grid-column-end: 2;
  }
  #item-2 {
    background-color: #ffede7;
    grid-row-start: 1;
    grid-column-start: 2;
    color: black;
    line-height: 350px;
    text-align: center;
    grid-row-end: 4;
    grid-column-end: 4;
  }
  #item-3 {
    background-color: #2cbccf;
    grid-row-start: 1;
    grid-column-start: 4;
    color: black;
    line-height: 105px;
    text-align: center;
    grid-row-end: 2;
    grid-column-end: 7;
  }
  #item-4 {
    background-color: #d870ed;
    grid-row-start: 4;
    grid-column-start: 1;
    color: black;
    line-height: 105px;
    text-align: center;
    grid-row-end: 5;
    grid-column-end: 4;
  }
  #item-5 {
    background-color: #edefc0;
    grid-row-start: 2;
    grid-column-start: 4;
    color: black;
    line-height: 220px;
    text-align: center;
    grid-row-end: 5;
    grid-column-end: 6;
  }
  #item-6 {
    background-color: #18b47b;
    grid-row-start: 2;
    grid-column-start: 6;
    color: black;
    line-height: 350px;
    text-align: center;
    grid-row-end: 5;
    grid-column-end: 7;
  }

  #squareOnTop {
    background: #293462;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 150px;
    width: 250px;
    position: relative;

  }

  .circle {
    height: 120px;
    width: 120px;
    border-radius: 50%;
    background: #fff1c1;
    position: relative;
    overflow: hidden;
  }

  .square {
    background: #fe5f55;
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

  @media only screen and (max-width: 550px) {
    .angry-grid {
      grid-template-columns: 1fr;
      grid-template-rows: 0.4fr 0.4fr 2.2fr 1.2fr 1.2fr 1.2fr 1fr;
      grid-template-areas:
        "div"
        "item-0"
        "item-1"
        "item-2"
        "item-3"
        "item-4"
        "item-5"
        "item-6"
        "main"
        "angry-grid";
    }
  }
</style>
