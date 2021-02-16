<template>
  <div>
    <b-form-select
      class="formselect"
      v-model="selected"
      :options="options"
    ></b-form-select>
  </div>
</template>

<script>
export default {
  name: "FormSelect",

  data() {
    return {
      selected: null,
      options: [
        { value: "64Kbps Mp3", text: "64Kbps Mp3" },
        { value: "320kbps MP3", text: "320kbps MP3" },
        { value: "256Kbps MP3", text: "256Kbps MP3" },
        { value: "192Kbps MP3", text: "192Kbps MP3" },
        { value: "128Kbps MP3", text: "128Kbps MP3" }
      ]
    };
  }
};
</script>

<style scoped>
.formselect {
  color: white;
  border-radius: 6px;
  border-bottom: none;
  height: 26px;
  background-color: #f7b263;
  border: none;
  padding: 0px 15px;
  width: 110px;
  margin-left: 15px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
