<template>
  <button class="Button">
    {{ text }}
  </button>
</template>

<
<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      required: true
    }
  },
  data(props) {
    const { text } = props;
    return {
      text
    };
  }
};
</script>

<style>
button {
  padding: 4px 15px;
  background: #ff0d0d;
  backdrop-filter: blur(20px);
  border-radius: 7px;
  width: 64px;
  color: white;
  border: none;
  height: 24px;
}
</style>
