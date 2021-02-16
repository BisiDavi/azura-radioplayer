<template>
  <b-container class="azuracast" fluid>
    <b-row class="align-items-center">
      <b-col cols="8">
        <Banner />
      </b-col>
      <b-col cols="1" class="divider"></b-col>
      <b-col cols="3">
        <Sidebar />
      </b-col>
    </b-row>
  </b-container>
</template>

<script>
export default {};
</script>

<style>
.azuracast {
  background-color: black;
  width: 100%;
  height: 100%;
  padding: 32px;
}
.divider {
  width: 2px;
  height: 100%;
  background: #2d2d2d;
  margin: 0px auto;
}
</style>
