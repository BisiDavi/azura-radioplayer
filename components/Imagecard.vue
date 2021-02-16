<template>
  <div class="imagecard">
    <img :src="video" alt="image" />
    <div class="text">
      <p>Travel and adventure</p>
      <h4>Radio station</h4>
    </div>
  </div>
</template>

<script>
export default {
  name: "Imagecard",
  data() {
    return {
      video
    };
  },
  props: {
    video: {
      type: String,
      required
    }
  }
};
</script>

<style scoped>
img {
  height: 300px;
  width: 300px;
}
.text {
  left: 15px;
  bottom: 20px;
  position: absolute;
  color: white;
  font-family: Poppins;
  font-style: normal;
}
p {
  font-weight: 500;
  font-size: 9px;
  line-height: 13p;
}
h4 {
  font-weight: bold;
  font-size: 18px;
  line-height: 27px;
  margin: 0px;
}
</style>
