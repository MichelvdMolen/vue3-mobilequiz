<template>
  <img
    id="win"
    class="quizimages"
    src="../assets/quizimage2.png"
    width="125"
    height="125"
  />
  <div id="winModal" class="modal">
    <div class="modal-content">
      <div class="correct"><h1>Congratulations!🥳</h1></div>
      <br />
      <img class="wonItem" src="../assets/winitem.jpg" />
      <p>You have won an Iphone X!</p>
      <button class="claimItem">
        <p>Click here to claim!</p>
        <p></p>
      </button>
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

.correct h1 {
  color: #44c767;
  font-family: "Open Sans", sans-serif;
}
p {
  font-family: "Open Sans", sans-serif;
}
.wonItem {
  height: 100px;
  width: auto;
}

.wonitem img {
  -webkit-animation: zoominandout 3s infinite;
  animation: zoominandout 3s infinite;
}

.claimItem {
  background-color: #44c767;
  border-radius: 12px;
  border: 1px solid #44c767;
  display: inline-block;
  cursor: pointer;
  color: #ffffff;
  font-family: Arial;
  font-size: 18px;
  padding: 0px 30px;
  text-decoration: none;
  -webkit-box-shadow: 0 5px 0 0 #359c51;
  -moz-box-shadow: 0 5px 0 0 #359c51;
  box-shadow: 0 5px 0 0 #359c51;
}
</style>
