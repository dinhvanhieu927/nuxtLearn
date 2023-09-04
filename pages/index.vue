<template>
  <div class="" style="min-height: 50vh">
    <h1></h1>
    <div class="home-content mt-2 flex justify-center">
      <div class="w-1/2">
        <canvas id="myCanvas" class="w-full" height="600" width="500" style="border:1px solid #d3d3d3;">
          Your browser does not support the HTML5 canvas tag.
        </canvas>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  mounted() {
    let c = document.getElementById("myCanvas");
    let ctx = c.getContext("2d");
    ctx.beginPath();
    ctx.strokeStyle = "#fff";
    ctx.moveTo(200, 200)
    ctx.lineTo(300, 250);
    ctx.stroke();

    ctx.beginPath();
    ctx.moveTo(200, 200)
    ctx.lineTo(200, 350);
    ctx.stroke();

    ctx.beginPath();
    ctx.moveTo(200, 350);
    ctx.lineTo(300, 400);
    ctx.stroke();

    ctx.beginPath();
    ctx.moveTo(300, 250);
    ctx.lineTo(300, 400);
    ctx.stroke();

    ctx.beginPath();
    ctx.moveTo(300, 250);
    ctx.lineTo(300, 400);
    ctx.stroke();
  }
}
</script>