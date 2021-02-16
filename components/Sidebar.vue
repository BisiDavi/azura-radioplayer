<template>
  <b-container class="sidebar">
    <b-row class="d-flex flex-column">
      <h3 class="mb-3">Other Playlist</h3>
      <div v-for="playlist in playlists" class="imagecards" :key="playlist.id">
        <Imagecard :imgsrc="playlist.image" />
      </div>
    </b-row>
  </b-container>
</template>

<script>
export default {
  name: "Sidebar",
  data() {
    return {
      playlists: [
        { id: 1, image: "/images/imageplaceholder5.png" },
        { id: 2, image: "/images/imageplaceholder4.png" },
        { id: 3, image: "/images/imageplaceholder3.png" },
        { id: 4, image: "/images/imageplaceholder2.png" },
        { id: 5, image: "/images/imageplaceholder5.png" },
        { id: 6, image: "/images/imageplaceholder4.png" },
        { id: 7, image: "/images/imageplaceholder3.png" },
        { id: 8, image: "/images/imageplaceholder2.png" }
      ]
    };
  }
};
</script>

<style scoped>
.sidebar {
  padding: 8px;
  overflow-y: auto;
  height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: black;
  margin: 10px;
}
p {
  margin-bottom: 4px;
}
img {
  margin: 5px;
}

h3 {
  color: white;
  font-family: Poppins;
  margin-left: 10px;
  text-align: left;
}
</style>
