<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/23/2020    Fixing the CSS
--->

<template>
  <div id="bottom_navbar"> 
   <div class="navbar-item">
          <h3 style="margin:-0.2vh">ScanTo3D</h3>
          <p style="font-size:1vw">@OPAL AI Inc 2020</p>
    </div>
    <div class="navbar-item">
        <p class="navbar-item" style="text-align:left">516 N Virgil Avenue<br>Los Angeles<br>California 50004</p>
    </div>
    <div class="navbar-item" style="text-align:left; line-height:30px"> 
      <i class="fas fa-phone-alt "></i> (323) 928-2029 <br>
      <a><i class="fas fa-envelope"></i> info@opaltech.ai</a>
    </div>
    <div class="navbar-item">
          <form class="form-inline my-2 my-lg-0 navbar-item">
            <input
              class="form-control mr-sm-2"
              type="email"
              placeholder="email"
              aria-label="Email" />
            <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
              Get download link
            </button>
          </form>
    </div>
    <div class="navbar-item" style="font-size:2vw">
            <i style="padding: 5px" class="fab fa-facebook" href="#"></i>
            <i style="padding: 5px" class="fab fa-twitter" href="#"></i>
            <i style="padding: 5px" class="fab fa-instagram" href="#"></i>
    </div>      
  </div>
</template>

<script>
export default {
  name: 'Footer',
  components: {},
};
</script>

<style>
#bottom_navbar {
  color: white !important;
  position: relative;
  width: 100%;
  background-color: #044790;
  padding: 1vw;
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
}

</style>
