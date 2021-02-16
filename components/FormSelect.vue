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
      selected: "64KBPS",
      options: [
        { value: "64KBPS", text: "64KBPS" },
        { value: "320KBPS", text: "320KBPS" },
        { value: "256KBPS", text: "256KBPS" },
        { value: "192KBPS", text: "192KBPS" },
        { value: "128KBPS", text: "128KBPS" }
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
  margin-left: 7px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
