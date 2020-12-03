<template>
<div>
  <b-navbar toggleable="lg" type="dark" variant="info">
    <img src="../assets/logo.png" href="/" class="d-inline-block align-top" alt="scan2plan logo">

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
          <b-nav-item>FIND AN ARCHITECT</b-nav-item>
          <b-nav-item>ORDER A SCAN</b-nav-item>
          <b-nav-item>Download the app</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>

<script>

export default {
  name: 'Navbar',
  components: {
    
  }
}
</script>