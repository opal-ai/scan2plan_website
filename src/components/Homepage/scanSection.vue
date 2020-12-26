<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div id="scan">
     <b-container>
      <b-row align-v="center">
        <b-col>
          <b-img fluid-grow :src="require('../../assets/3d_model.png')" id="modelImage"></b-img>
        </b-col>
        <b-col cols="auto">
          <p style="margin-top:7vh; font-size:2.5rem; font-weight:bolder; padding:10px">SCHEDULE A SCAN</p>
          <p class="floor_p"> Select a date/time and someone from our team <br> will be there to do the rest </p>
          <button
            type="button"
            id="scanButton"
            href="#"
            style="margin-bottom:5vh"
            v-b-modal.scanInfoModal
          >
            Schedule Scan
          </button>

          <b-modal id="scanInfoModal">
                <!-- <button class="modalButton" v-on:click="showArchitectLogin">Find an Architect</button>
                <button class="modalButton">Find a project</button> -->
                <h3>Coming soon!</h3>
                <p> You can now have someone come to your home and take measurements in just a click.
                  Select a date and time that suits you and a member from our team will be there to take all the measurements.
                </p>
              </b-modal>
        </b-col>
      </b-row>
    </b-container>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'ScanSection',
  components: {},
};
</script>

<style scoped>
  #scan{
  width:100%
  }

.floor_p {
  margin-top: 1vh;
  font-size: 1.5rem;
  line-height: 30px;
}

#scanButton{
    background-color: #044790;
    padding: 7px;
    border-radius: 10px;
    font-size: 0.75rem;
    color:white;
    width: 50%;
    font-size: 1.2rem;
    margin-top: 1vh
  }

#modelImage{
  max-width: 90%;
  margin-bottom: 3vh
}

</style>
