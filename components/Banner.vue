<template>
  <b-container class="banner">
    <b-row cols="2" class="justify-content-between align-items-center">
      <b-col lg="6" class="d-flex align-items-center">
        <b-row class="align-items-center">
          <b-col lg="4">
            <Thumbnailcard
              imgsrc="/images/imageplaceholder1.png"
              height="100px"
              width="100px"
              :play="false"
            />
          </b-col>
          <b-col lg="8">
            <span class="d-flex flex-column">
              <h5>Radio station playlist</h5>
              <p>Travel and adventure</p>
            </span>
          </b-col>
        </b-row>
      </b-col>
      <b-col lg="1">
        <img src="/images/heart.png" class="heartIcon" alt="heart" />
      </b-col>
    </b-row>
  </b-container>
</template>

<style scoped>
h5,
p {
  font-family: "Poppins";
  font-weight: "normal";
}
h5 {
  color: white;
  font-size: 18px;
  line-height: 27px;
  font-weight: 500;
}
p {
  font-size: 12px;
  color: #484848;
  line-height: 18px;
}
img.heartIcon {
  padding: 15px;
  border: 1px solid #ff8a00;
  box-sizing: border-box;
  border-radius: 8px;
  display: flex;
  align-items: center;
  justify-content: center;
}
</style>
