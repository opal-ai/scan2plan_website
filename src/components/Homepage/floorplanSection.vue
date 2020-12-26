<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div id="floorplan">
    <b-container>
      <b-row align-v="center">
        <b-col>
          <b-img fluid-grow :src="require('../../assets/devices.png')" id="devicesImage"></b-img>
        </b-col>
        <b-col cols="auto">
          <p style="margin-top:7vh; font-size:2.5rem; font-weight:bolder; padding:10px">GET A FLOORPLAN</p>
          <p class="floor_p">
            Need an instant 3D Model of your home? <br>
            Need a floor plan, without the hassle? <br> 
            Need an architect? </p>
            <p style="font-size: 1.7rem; margin-top:1vh"> We have it all covered! </p>
          <a :href="url">
            <div
              id="downloadButton">
              Download the app
            </div>
          </a>  
        </b-col>
      </b-row>
    </b-container>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'FloorplanSection',
  components: {},
  data: function(){
    return {
      url: 'https://apps.apple.com/us/app/scanto3d/id1537506295'
    }
  }
};
</script>

<style scoped>

#floorplan{
  width:100%
}

.floor_p {
  margin-top: 1vh;
  font-size: 1.5rem;
  line-height: 30px;
}

#devicesImage{
  max-width: 80%;
}

#downloadButton{
  background-color: #044790;
  padding: 7px;
  border-radius: 10px;
  color:white;
  width: 50%;
  font-size: 1.2rem;
  margin: 1vh auto 3vh auto;
}

</style>
