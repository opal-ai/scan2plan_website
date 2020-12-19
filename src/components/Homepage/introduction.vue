<!-- @format -->

<template>
  <div class="introduction">
    <div class="bg"></div>
    <b-container>
      <b-row align-h="around" align-v="center">
        <b-col cols="5">
          <h1 class="intro_title" style="margin-top: 10vh">SCAN2PLAN</h1>
          <p class="intro_p">Need an instant 3D Model of your home?</p>
          <p class="intro_p">Need a floorplan, without the hassle?</p>
          <p class="intro_p">Need an architect?</p>
          <h4 style="color:black">We have it all covered!</h4>
          <p
            style="text-decoration: underline; margin-bottom: 10vh; color: #007bfe"
          >
            Learn More
          </p>
        </b-col>
        <b-col cols="7">
          <img src="../../assets/phone.png" width="300vw" height="100%" />
        </b-col>
      </b-row>
    </b-container>

    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'Introduction',
  components: {},
};
</script>

<style>
.introduction {
  position: relative;
  z-index: 1;
  width: 100%;
}
.introduction .bg {
  position: absolute;
  z-index: -1;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  background-image: url('../../assets/alimo.png');
  background-repeat: no-repeat;
  /* background-size: 40vw 80vh; */
  height: 100%;
  background-size: cover;
  width: 100%;
  background-position: center;
  opacity: 0.3;
}
.intro_p {
  margin: -3px;
  color: black;
  font-weight: bold;
}
.intro_title {
  color: #007bfe;
}
</style>
