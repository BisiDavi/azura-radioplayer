<template>
  <div class="videocard my-2">
    <img :src="videosrc" width="100%" height="350px" />
    <div class="btnGrp">
      <Button text="Live" />
      <Iconbutton text="8/10" iconImg="/images/profile.png" />
    </div>
    <img src="/images/play.png" alt="play icon" class="playIcon" />
  </div>
</template>

<script>
export default {
  name: "Videocard",
  props: {
    videosrc: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.videocard {
  position: relative;
}
.playIcon {
  position: absolute;
  top: 40%;
  left: 45%;
}
h3 {
  color: white;
  font-family: 'Poppins', sans-serif;
  margin-left: 10px;
  text-align: left;
}
.btnGrp {
  display: flex;
  position: absolute;
  top: 20px;
  left: 40px;
  width: 160px;
  justify-content: space-between;
  align-items: center;
}
</style>
