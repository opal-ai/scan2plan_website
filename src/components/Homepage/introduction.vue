<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div class="introduction">
    <div class="bg"></div>
    <b-row align-v="center" class="minSectionHeight">
        <b-col cols="4" id="rhsSection" >
          <div style="position: absolute; bottom: 0; left: 0">
                <img src="../../assets/phone.png" id="introImage" />
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

#introImage{
 width:34vw; 
 float:left;
}

@media only screen and (max-width: 600px){
  #introImage{
    width:50vw; 
    float:left;
}
}

#rhsSection{
  min-height: 50vh !important;
  padding: 0px;
}
</style>
