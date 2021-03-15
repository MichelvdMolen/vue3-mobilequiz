<template>
  <Header></Header>
  <Prize></Prize>
  <Select></Select>
  <QuizImages></QuizImages>
  <QuizImages></QuizImages>
  <Winimage></Winimage>
  <QuizImages></QuizImages>
  <Footer></Footer>
</template>

<script>
import Header from "./components/Header.vue";
import Prize from "./components/Prize.vue";
import QuizImages from "./components/QuizImages.vue";
import Winimage from "./components/Winimage.vue";
import Select from "./components/Select.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Prize,
    QuizImages,
    Winimage,
    Select,
    Footer,
  },
};

window.onload = function() {
  var winmodal = document.getElementById("winModal");
  var losemodal = document.getElementById("loseModal");

  var winimage = document.getElementById("win");
  var loseimage = document.getElementById("lose");

  winimage.onclick = function() {
    winmodal.style.display = "block";
  };
  loseimage.onclick = function() {
    losemodal.style.display = "block";
  };

  window.onclick = function(event) {
    if (event.target == winmodal || event.target == losemodal)
      (winmodal.style.display = "none"), (losemodal.style.display = "none");
  };
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@700&display=swap");
body {
  background: #dadaff;
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.modal {
  display: none;
  position: fixed;
  z-index: 1;
  padding-top: 100px;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgb(0, 0, 0);
  background-color: rgba(0, 0, 0, 0.4);
}

.modal-content {
  background: rgb(54, 51, 101);
  background: linear-gradient(
    0deg,
    rgba(54, 51, 101, 1) 0%,
    rgba(222, 222, 222, 1) 0%,
    rgba(255, 255, 255, 1) 100%
  );
  margin: auto;
  padding: 20px;
  border: 1px solid #888;
  width: 80%;
}
</style>
