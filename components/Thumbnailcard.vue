<template>
  <div class="thumbnail">
    <div
      img-src="require(`~assets/images/${thumbnailImg}.png`)"
      alt="thumbnail"
      img-height="height"
      img-width="width"
    ></div>
  </div>
</template>

<script>
export default {
  name: "Thumbnailcard",
  props: {
    thumbnailImg: {
      type: String,
      required: true
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
.thumbnail {
  margin: "10px";
}
</style>
