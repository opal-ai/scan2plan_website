<!-- @format -->

<template>
  <div id="floorplan">
    <b-container>
      <b-row>
        <b-col>
          <img src="../../assets/devices.png" width="300vw" height="90%" />
        </b-col>
        <b-col cols="auto">
          <h3 style="margin-top:7vh">GET A FLOORPLAN</h3>
          <!-- <b-container>
            <b-row align-v="left"> -->
          <p class="floor_p">
            Our app is the one stop solution to all your home planning problems.
          </p>
          <p class="floor_p">
            Get an instant 3D model, request a professional AutoCAD floorplan
            and more!
          </p>
          <!-- </b-row>
          </b-container> -->
          <button
            type="button"
            class="btn btn-primary"
            href="#"
            style="margin-bottom:5vh; margin-top:5px"
          >
            Download the app
          </button>
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
};
</script>

<style>
.floor_p {
  margin: -5px;
  font-weight: bold;
}
</style>
