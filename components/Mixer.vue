<template>
  <div class="mixer d-flex flex-column mt-4 p-3">
    <p class="my-3">Volume mixer</p>
    <span class="volume-controls">
      <Slider :showControls="true" />
    </span>
    <div class="volume-mixer d-flex my-3 mx-0">
      <span class="sound mr-4">
        <p class="mt-0 mb-4 mr-4">Quality sounds</p>
        <div class="d-flex align-items-center justify-content-between">
          <img class="mr-2" src="/images/play-min.png" alt="play icon" />
          <FormSelect />
        </div>
      </span>
      <span class="playlist">
        <p class="mt-0 mb-4">Playlist song</p>
        <button class="download">
          Download <img src="/images/download.png" class="ml-2" alt="icon" />
        </button>
      </span>
    </div>
  </div>
</template>

<script>
export default {
  name: "Mixer"
};
</script>

<style scoped>
.mixer {
  width: 100%;
  height: 208px;
  background: #ff8a00;
  border-radius: 18px;
  display: flex;
  color: white;
  justify-content: flex-start;
  flex-direction: column;
  padding: 10px 25px;
}
p {
  color: white;
  font-family: Poppins;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 21p;
}
.volume-mixer {
  display: flex;
  width: 100%;
}
.playlist,
.sound {
  display: flex;
  flex-direction: column;
  width: 160px;
}

.sound {
  justify-content: flex-start;
}

.volume-controls input {
  width: 85% !important;
}

button.download {
  display: flex;
  justify-content: center;
  padding: 4px 7px;
  background: #f7b263;
  border-radius: 6px;
  width: 175px;
  align-items: center;
  color: white;
  border: none;
  height: 28px;
}
input {
  width: 85% !important;
}

img {
  margin: 2px 5px;
}
</style>
