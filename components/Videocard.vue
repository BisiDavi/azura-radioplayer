<template>
  <div class="videocard">
    <img :src="video" width="900px" height="350px" />
    <div class="btnGrp">
      <Button text="Live" />
      <Iconbutton text="8/10" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Videocard",
  props: {
    videosrc: {
      type: String,
      required: true
    }
  },
  data(props) {
    const { videosrc } = props;
    return {
      videosrc
    };
  }
};
</script>

<style scoped>
h3 {
  color: white;
  font-family: Poppins;
  margin-left: 10px;
  text-align: left;
}
</style>
