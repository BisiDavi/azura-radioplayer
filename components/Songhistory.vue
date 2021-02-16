<template>
  <div class="song-history">
    <h3>
      Song <br />
      History
    </h3>
    <span
      v-bind="images"
      v-for="img in imagesArray"
      :key="img.id"
      class="imgGrp"
    >
      <Thumbnail imgsrc="img.image" height="120" width="160" play />
    </span>
  </div>
</template>

<script>
export default {
  name: "Songhistory",
  data() {
    return {
      imagesArray: [
        { id: 1, image: "/imageplaceholder8.png" },
        { id: 2, image: "/imageplaceholder7.png" },
        { id: 3, image: "/imageplaceholder6.png" }
      ]
    };
  }
};
</script>
