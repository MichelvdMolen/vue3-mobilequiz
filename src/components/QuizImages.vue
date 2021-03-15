<template>
  <img
    id="lose"
    class="quizimages"
    src="../assets/quizimage.png"
    width="125"
    height="125"
  />
  <div id="loseModal" class="modal">
    <div class="modal-content">
      <div class="wrong"><h1>Too bad, try again!😔</h1></div>
    </div>
  </div>
</template>

<style>
.quizimages {
  margin: 10px;
  border: 5px solid #00abff;
  -webkit-box-shadow: 0px 2px 5px 0px rgba(154, 157, 183, 1);
  -moz-box-shadow: 0px 2px 5px 0px rgba(154, 157, 183, 1);
  box-shadow: 0px 2px 5px 0px rgba(154, 157, 183, 1);
  border-radius: 15px;
  cursor: pointer;
}

.quizimages:hover {
  -webkit-transform: scale(1.2);
  -ms-transform: scale(1.2);
  transform: scale(1.2);
  border: 5px solid #0068ff;
}

.wrong h1 {
  color: #6b0000;
  font-family: "Open Sans", sans-serif;
}

@keyframes zoominandout {
  0% {
    transform: scale(1, 1);
  }
  30% {
    transform: scale(1.05, 1.05);
  }

  100% {
    transform: scale(1, 1);
  }
}

img {
  animation: zoominandout 6s infinite;
}
</style>
