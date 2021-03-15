<template>
  <div class="winItem">
    <div class="winElement">
      <img
        src="../assets/winitem.jpg"
        width="50"
        height="75"
        class="winImageItem"
      />
      <h3>
        Find the different picture!
      </h3>
      <h4>
        And win an <span>{{ prize }}</span>
      </h4>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      prize: "Apple iPhone 12 Pro Max!",
    };
  },
};
</script>

<style>
.winElement {
  height: 110px;
  width: 90%;
  margin: auto;
  background-color: white;
  margin-top: 10%;
  -webkit-box-shadow: 0px 2px 5px 0px rgba(154, 157, 183, 1);
  -moz-box-shadow: 0px 2px 5px 0px rgba(154, 157, 183, 1);
  box-shadow: 0px 2px 5px 0px rgba(154, 157, 183, 1);
  border-radius: 15px;
  text-align: left;
}

.winItem img {
  float: left;
  padding: 10px;
  display: flex;
  animation: bounce 2s infinite;
  margin-top: 10px;
}

.winItem h3 {
  padding-top: 10px;
  color: #0068ff;
}

.winItem h4 {
  font-size: 18px;
  margin: 10px;
}

.bounce {
  animation: bounce 1.5s infinite;
}

@keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-10px);
  }
  60% {
    transform: translateY(-5px);
  }
}
</style>
