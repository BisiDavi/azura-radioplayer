<template>
  <b-container>
    <b-row class="volume-slider">
      <b-icon v-if="showControls === true" icon="volume-off"></b-icon>
      <b-form-input type="range"></b-form-input>
      <b-icon v-if="showControls === true" icon="volume-up"></b-icon>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Slider",
  props: {
    showControls: {
      type: Boolean,
      required: true
    }
  }
};
</script>

<style scoped>
.volume-slider {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
