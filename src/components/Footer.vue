<template>
  <div class="text">
    <!--<h2>Play and win!</h2>-->
    <h2><span>Play</span><span>&</span><span>win!</span></h2>
  </div>
</template>

<script>
export default {};
</script>

<style>
h2 {
  margin: 0;
  font-size: 40px;
  padding: 0;
  color: #2c3e50;
  margin-top: 10%;
  font-family: "Open Sans", sans-serif;
}
span {
  transform: scale(0.9);
  display: inline-block;
  font-family: "Open Sans", sans-serif;
}
span:first-child {
  animation: bop 1s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards infinite
    alternate;
}
span:last-child {
  animation: bopB 1s 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275) forwards
    infinite alternate;
}

@keyframes bop {
  0% {
    transform: scale(0.9);
  }
  50%,
  100% {
    transform: scale(1);
  }
}

@keyframes bopB {
  0% {
    transform: scale(0.9);
  }
  80%,
  100% {
    transform: scale(1) rotateZ(-3deg);
  }
}
</style>
