<template>
  <button class="Button">
    <img :src="iconimg" alt="icon" height="15px" width="15px" />
    {{ text }}
  </button>
</template>

<
<script>
export default {
  name: "Iconbutton",
  props: {
    text: {
      type: String,
      required: true
    },
    iconimg: {
      type: String,
      required: true
    }
  },
  data(props) {
    const { text, iconimg } = props;
    return {
      text,
      iconimg
    };
  }
};
</script>

<style>
button {
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
}
img {
  margin: 2px 5px;
}
</style>
