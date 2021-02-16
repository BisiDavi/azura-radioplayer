<template>
  <div class="imagecard">
    <img :src="imgsrc" alt="image" />
    <div class="text">
      <p>Travel and adventure</p>
      <h4>Radio station</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "Imagecard",
  props: {
    imgsrc: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.imagecard {
  position: relative;
}
img {
  height: 190px;
  width: 220px;
  margin: 10px;
}
.text {
  left: 25px;
  bottom: 20px;
  position: absolute;
  color: white;
  font-family: Poppins;
  font-style: normal;
}
p {
  font-weight: 500;
  font-size: 9px;
  line-height: 13px;
  margin: 0px;
}
h4 {
  font-weight: bold;
  font-size: 18px;
  line-height: 27px;
  margin: 0px;
}
</style>
