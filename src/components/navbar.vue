<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
--->

<template>
  <div>
    <b-navbar toggleable="lg" type="light" variant="light">
      <img
        src="../assets/logo.png"
        href="/"
        class="d-inline-block align-top logo"
        alt="scan2plan logo"
      />

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item
            ><a href="#" class="blue-text nav-link"
              >FIND AN ARCHITECT</a
            ></b-nav-item
          >
          <b-nav-item
            ><a href="#" class="blue-text nav-link">ORDER A SCAN</a></b-nav-item
          >
          <b-nav-item
            ><button type="button" class="btn btn-primary" href="#">
              Download the app
            </button></b-nav-item
          >
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  components: {},
};
</script>
<style scoped>
/* .navbar {
  background-color: white;
} */
.blue-text {
  color: #007bfe !important;
}
.white-button {
  color: white;
  background-color: blue;
  border-radius: 50px;
}
.logo {
  width: 13vh;
  height: 5vw;
}

</style>
