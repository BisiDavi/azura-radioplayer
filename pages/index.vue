<template>
  <b-container class="azuracast" fluid>
    <b-row class="mx-auto pagerow">
      <b-col class="content px-5" cols="9">
        <Banner />
        <Videocard videosrc="/images/videoplaceholder.png" />
        <b-row class="mt-4">
          <b-col cols="6">
            <Mediaplayer />
          </b-col>
          <b-col class="d-flex flex-column" cols="6">
            <Songhistory />
            <Mixer />
          </b-col>
        </b-row>
      </b-col>
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
.pagerow {
  position: relative;
}
.content:after {
  width: 4px;
  position: absolute;
  height: 100%;
  background: #2d2d2d;
  content: "";
  top: 0px;
  right: 10px;
  border-radius: 15px;
}
</style>
