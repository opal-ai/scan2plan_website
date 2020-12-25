<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/23/2020    Fixing the CSS
--->

<template>
  <div id="bottom_navbar"> 
   <div class="navbar-item">
          <p style="margin:-0.2vh; font-size:1.5rem">ScanTo3D</p>
          <p style="font-size:0.5rem">@OPAL AI Inc 2020</p>
    </div>
    <div>
        <p class="navbar-item"> <b>OPAL AI Inc</b> <br> </p>
        <p class="navbar-item" style="font-size: 0.75rem; margin-top:3px"> 516 N Virgil Avenue<br>Los Angeles<br>California 50004</p>
    </div>
    <div class="navbar-item" style="line-height:30px"> 
      <i class="fas fa-phone-alt "></i> (323) 928-2029 <br>
      <a><i class="fas fa-envelope"></i> info@opaltech.ai</a>
    </div>
    <div class="navbar-item" style="font-size:1.75rem">
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
  display: grid;
  grid-template-columns: auto auto auto auto;
  align-items: center;
  justify-content: space-between;
}

.navbar-item{
  text-align: left;
}

@media only screen and (max-width: 600px){
  #bottom_navbar {
    grid-template-columns: auto;
    justify-content: center;
    grid-gap: 2vh;
  }

  .navbar-item{
     text-align: center;
  }
}
</style>
