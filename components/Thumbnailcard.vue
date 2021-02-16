<template>
  <div class="thumbnailcard">
    <b-img
      alt="thumbnail"
      class="thumbnail"
      :src="imgsrc"
      :height="height"
      :width="width"
    ></b-img>
    <div class="play-icon" v-if="play === true">
      <img src="/images/play-min.png" alt="play icon" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Thumbnailcard",
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
