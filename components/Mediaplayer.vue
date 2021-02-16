<template>
  <b-card class="mediaplayer px-1">
    <b-card-header class="d-flex header mt-0 py-2 px-2">
      <Thumbnailcard
        imgsrc="/images/imageplaceholder1.png"
        height="100px"
        width="100px"
        :play="false"
      />
      <div class="text">
        <p>Travel and adventure</p>
        <h3>Radio station</h3>
      </div>
    </b-card-header>
    <b-card-body class="px-0">
      <img src="/images/wave.png" alt="wave" height="100px" width="100%" />
    </b-card-body>
    <b-card-footer class="footer px-0">
      <Slider />
      <div :key="control.id" v-for="control in contols">
        <img :src="control.image" :class="playPause(control)" />
      </div>
    </b-card-footer>
  </b-card>
</template>

<script>
export default {
  name: "Mediaplayer",
  data() {
    return {
      controls: [
        { id: 1, image: "/images/shuffle.svg" },
        { id: 2, image: "/images/prev.png" },
        { id: 3, image: "/images/pause.png" },
        { id: 4, image: "/images/next.png" },
        { id: 5, image: "/images/repeat.png" }
      ]
    };
  },
  methods: {
    playPause(control) {
      const controlState = control.image.includes("/pause.png")
        ? "pauseIcon"
        : "controlsIcon";
      return controlState;
    }
  }
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

.controlsIcon {
  margin: 0px 25px;
}
.pauseIcon {
  background: linear-gradient(180deg, #fa5c03 0%, #e12a2a 100%);
  padding: 20px 15px 10px 15px;
  border-radius: 50%;
  margin: 0px 10p;
}
.text {
  font-family: Poppins;
  font-style: normal;
  margin-left: 10px;
}
.header,
.footer {
  border: none;
}

.mediaplayer {
  background-color: #232323;
  border-radius: 18px;
  color: white;
  font-family: Poppins;
  padding: 21px;
  height: 385px;
}
h3 {
  font-size: 30px;
  line-height: 50px;
  margin: 0p;
}
p {
  font-weight: 500;
  font-size: 14px;
  line-height: 21px;
  color: #5f5f5f;
  margin: 0p;
}
</style>
