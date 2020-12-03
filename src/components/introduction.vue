<template>
  <div id="introduction">
      <!-- <b-container fluid> -->
        <b-row align-h="around" align-v="center">
            <b-col cols="5">
                <h3>SCAN2PLAN</h3>
                <p>Need an instant 3D Model of your home?</p>
                <p>Need a floorplan, without the hassle?</p>
                <p>Need an architect?</p>
                <h3>We have it all covered!</h3>
                <p style="text-decoration: underline;">Learn More</p>
            </b-col>
            <b-col cols="7">
                <img src="../../src/assets/phone.png" width="300vw" height="200vw"/>
            </b-col>
        </b-row>
      <!-- </b-container> -->
    
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name:"Introduction",
  components: {
  },
}
</script>


<style>
#introduction {
  background-image: url('../../src/assets/alimo.png');
  background-repeat: no-repeat;
  background-size: 40vw 80vh;
}
</style>