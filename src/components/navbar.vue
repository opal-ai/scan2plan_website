<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div>
    <b-navbar toggleable="lg" type="light" id="navbar">
      <b-navbar-brand href="#">
        <img src="../assets/opal_logo_50.png" href="#" class="d-inline-block align-top logo" alt="scan2plan logo"/>
      </b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>
         <b-navbar-nav class="ml-auto">
          <b-nav-item v-bind:href="url" class="blue-text">
              ARCHITECT CONNECT
           </b-nav-item>
          <b-nav-item v-bind:href="url" class="blue-text">
            ORDER A SCAN
            </b-nav-item>
          <b-nav-item v-bind:href="url">
              <div id="downloadButton"> Download the app</div>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  data: function(){
    return {
      url: 'https://apps.apple.com/us/app/scanto3d/id1537506295'
    }
  },
  components: {},
};
</script>
<style scoped>
.blue-text a{
  color: #044790 !important;
  font-size: 0.75rem;
  margin-top: 7px;
}

#downloadButton{
  background-color: #044790;
  padding: 7px;
  border-radius: 10px;
  font-size: 0.75rem;
  color:white
}

</style>
