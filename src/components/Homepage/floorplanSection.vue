<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div id="floorplan">
    <b-container>
      <b-row>
        <b-col>
          <b-img fluid-grow :src="require('../../assets/devices.png')" id="devicesImage"></b-img>
        </b-col>
        <b-col cols="auto">
          <p style="margin-top:7vh; font-size:2.5rem; font-weight:bolder">GET A FLOORPLAN</p>
          <p class="floor_p">
            ScanTo3D is the one stop solution to all your home planning problems.
          </p>
          <p class="floor_p">
            Get an instant 3D model, request a professional AutoCAD floorplan
            and more!
          </p>
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

<style>

#floorplan{
  margin-top: 5vh;
  width:100%
}

.floor_p {
  font-size: 1rem;
}

#devicesImage{
  max-width: 80%;
}

#downloadButton{
  background-color: #044790;
  padding: 7px;
  border-radius: 10px;
  font-size: 0.75rem;
  color:white;
  width: 50%;
  font-size: 1.2rem;
  margin: 3vh auto 3vh auto;
}

</style>
