<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div class="introduction">
    <div class="bg"></div>
    <b-row align-v="center">
        <!-- <b-col cols="8">
          <b-row>
            <b-col cols="6">
              <h1 class="intro_title" style="margin-top: 10vh">OPLAN</h1>
              </b-col>
            <b-col cols="6">
              <div id="taglines">
                <p class="intro_p">Need an instant 3D Model of your home?</p>
                <p class="intro_p">Need a floorplan, without the hassle?</p>
                <p class="intro_p">Need an architect?</p>
                <h4 style="color:black; font-size: 2em; ">Our app has it all covered!</h4>
                <p style="text-decoration: underline; margin-bottom: 10vh; color: #007bfe">Learn More</p>
              </div>
            </b-col>
          </b-row>
        </b-col>
        <b-col cols="4" style="padding:0px" id="imageDiv">
          <img src="../../assets/phone.png" style="width:30vw; float:right"/>
        </b-col> -->
        <!--SECOND WAY -->
        <b-col cols="4" id="rhsSection" >
          <div style="position: absolute; bottom: 0; left: 0">
                <img src="../../assets/phone.png" style="width:32vw; float:left"/>
          </div>
        </b-col>
        <b-col cols="8">
          <div style="text-align: left">
            <p style="color: black">OPAL AI presents</p>
            <h1 class="intro_title">ScanTo3D</h1>
          </div>
          <div id="taglines">
            <p style="padding-left: 6vw">Instant 3D Models, floor plans, quick access to architects and more</p>
          </div>
          
        </b-col >
      </b-row>
  </div>
</template>

<script>
export default {
  name: 'Introduction',
  components: {},
};
</script>

<style>

p{
  margin-bottom: -5px;
}

.introduction {
  position: relative;
  z-index: 1;
  width: 100%;
}
.introduction .bg {
  position: absolute;
  z-index: -3;
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
  opacity: 0.2;
}

#taglines{
  padding-right: 5px;
  margin-top: -2vh;
  font-size: 1.5vw;
  text-align: left;
  font-weight: bold;
}

.intro_p {
  color: black;
  font-size: 1.5em;
  line-height: 20px;
}
.intro_title {
  font-weight: bolder;
  font-size: 8vw;
  color: #044790;
}

#imageDiv{
  padding: 0px;
  position: absolute;
  right: 0;
  bottom: 0
}

#rhsSection{
  min-height: 40vh !important;
}
</style>
