<template>
  <button class="Button">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: {
      type: String,
      required: true
    }
  }
};
</script>

<style>
button.Button {
  padding: 4px 15px;
  background: #ff0d0d;
  backdrop-filter: blur(20px);
  border-radius: 7px;
  width: 64px;
  color: white;
  justify-content: center;
  border: none;
  height: 24px;
  display: flex;
  align-items: center;
}
</style>
