<template>
  <div class="thumbnailcard">
    <b-img alt="thumbnail" class="thumbnail" v-bind="cardProps"></b-img>
    <div class="play-icon" v-if="play">
      <img src="/images/play.png" alt="play" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Thumbnailcard",
  data(props) {
    const { width, height, imgsrc, play } = props;
    return {
      cardProps: {
        width: width,
        height: height,
        src: imgsrc
      },
      play
    };
  },
  props: {
    imgsrc: {
      type: String,
      required: true
    },
    play: {
      type: Boolean
    },
    height: {
      type: String,
      required: true
    },
    width: {
      type: String,
      required: true
    }
  }
};
</script>

<style scoped>
.thumbnailcard {
  margin: "10px";
}
</style>
