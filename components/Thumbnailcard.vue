<template>
  <div>
    <b-card img-src="require(`~assets/images/${thumbnailImg}.png`)" alt="thumbnailAlt"> </b-card>
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
    thumbnailAlt: {
      type: String,
      required: true
    }
  }
};
</script>
