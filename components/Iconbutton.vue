<template>
  <button class="Iconbutton">
    <img :src="iconImg" alt="icon" height="15px" width="15px" />
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Iconbutton",
  props: {
    text: {
      type: String,
      required: true
    },
    iconImg: {
      type: String,
      required: true
    }
  }
};
</script>

<style>
button.Iconbutton {
  display: flex;
  justify-content: space-around;
  padding: 4px 7px;
  background: rgba(0, 0, 0, 0.25);
  backdrop-filter: blur(20px);
  border-radius: 7px;
  width: 70px;
  color: white;
  border: none;
  height: 24px;
  justify-content: center;
  display: flex;
  align-items: center;
}
img {
  margin: 2px 5px;
}
</style>
