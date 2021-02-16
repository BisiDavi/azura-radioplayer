<template>
  <div class="songhistory">
    <h3>
      Song <br />
      History
    </h3>
    <span v-for="img in imagesArray" :key="img.id" class="imgGrp">
      <Thumbnailcard :imgsrc="img.image" height="120" width="160" :play="true" />
    </span>
  </div>
</template>

<script>
export default {
  name: "Songhistory",
  data() {
    return {
      imagesArray: [
        { id: 1, image: "/imageplaceholder8.png" },
        { id: 2, image: "/imageplaceholder7.png" },
        { id: 3, image: "/imageplaceholder6.png" }
      ]
    };
  }
};
</script>

<style scoped>
.songhistory {
  height: 145px;
  width: 100%;
  padding: 15px 20px 10px 20px;
  background-color: #292929;
  border-radius: 15px;
  display: flex;
  align-items: center;
}
h3 {
  color: white;
  font-family: Poppins;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 116.5%;
}
.imggrp {
  margin-left: 20px;
  display: flex;
  align-items: center;
}
img {
  margin: 6px;
}
</style>
