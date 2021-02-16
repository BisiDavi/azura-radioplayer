<template>
  <div class="imagecard">
    <img :src="require(`~/assets/images/${video}`)" alt="image" />
  </div>
</template>

<script>
export default {
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
</style>
