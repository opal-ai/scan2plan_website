<!-- @format -->

<template>
  <div id="bottom_navbar">
    <nav class="navbar navbar-expand-lg navbar-light bg-primary">
      <a class="navbar-brand" href="#">
        <h4 style="margin:-0.2vh">SCAN2PLAN</h4>
        <p>@OPAL AI Inc 2020</p>
      </a>

      <button
        class="navbar-toggler"
        type="button"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <i class="fas fa-search-location"
              ><p>516 N Virgil Avenue</p>
              <p>Los Angeles</p>
              <p>California 90004</p>
            </i>
          </li>
          <b-container>
            <li class="nav-item">
              <b-row>
                <i class="fas fa-envelope-square"
                  ><a class="nav-link" href="#">info@opaltech.ai</a></i
                >
              </b-row>
              <b-row>
                <i class="fas fa-phone"
                  ><a class="nav-link disabled" href="#">(323) 928-2029</a></i
                >
              </b-row>
            </li>
          </b-container>
        </ul>

        <form class="form-inline my-2 my-lg-0">
          <input
            class="form-control mr-sm-2"
            type="email"
            placeholder="email"
            aria-label="Email"
          />
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">
            Get download link
          </button>
        </form>
        <!-- add fontawesome ican for facebook, twitter, and instagram -->
        <i class="fab fa-facebook" href="#"></i>
        <i class="fab fa-twitter" href="#"></i>
        <i class="fab fa-instagram" href="#"></i>
      </div>
    </nav>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'BottomNavbar',
  components: {},
};
</script>

<style>
#bottom_navbar {
  color: black !important;
}
</style>
