<template>
  <div class="thumbnailcard">
    <b-img alt="thumbnail" class="thumbnail" v-bind="cardProps"></b-img>
  </div>
</template>

<script>
export default {
  name: "Thumbnailcard",
  data(props) {
    return {
      cardProps: {
        width: props.cardWidth,
        height: props.cardHeight,
        src: props.thumbnailImg
      }
    };
  },
  props: {
    thumbnailImg: {
      type: String,
      required: true
    },
    cardHeight: {
      type: String,
      required: true
    },
    cardWidth: {
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
