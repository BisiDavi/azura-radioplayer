<template>
  <b-card>
    <b-card-header class="d-flex header">
      <Thumbnailcard />
      <p>Travel and adventure</p>
      <h3>Radio station</h3>
    </b-card-header>
    <b-card-body>
      <img src="~assets/images/wave.png" alt="wave" />
    </b-card-body>
    <b-card-footer>
      
    </b-card-footer>
  </b-card>
</template>

<script>
export default {
  name: "Mediaplayer"
};
</script>

<style scoped>
.header {
  font-family: Poppins;
  font-style: normal;
  margin-left: 10px;
}
h3 {
  font-size: 30px;
  line-height: 50px;
  margin: 0px;
}
p {
  font-weight: 500;
  font-size: 14px;
  line-height: 21px;
  color: #5f5f5f;
  margin: 0px;
}
img {
  height: 200px;
  width: 500px;
}
</style>
