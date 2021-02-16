<template>
  <button class="Button">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Dropdownbutton",
  props: {
    text: {
      type: String,
      required: true
    },
    options:{
      type: Array,
    }
  },
  data(props) {
    const { text, options } = props;
    return {
      text,
      options
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
