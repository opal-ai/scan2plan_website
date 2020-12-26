<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/19/2020    Adding Connect Architect functionality
--->
<template>
  <div id="app">
    <Navbar />
    <!--V1.1 changes start -->
    <div id="mainContent">
      <Homepage @showInterface="updatePage" v-if="showPage === 'homepage'"/>
      <FindArchitect v-if="showPage === 'architect'"/>
    </div>
    <!--V1.1 changes end -->
    <Footer />
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap-vue/dist/bootstrap-vue.css';
import Vue from 'vue';
import { BootstrapVue } from 'bootstrap-vue';
import Homepage from './components/Homepage/homepage';
import Navbar from './components/navbar.vue';
import Footer from './components/footer.vue';
import FindArchitect from './components/Architect/findArchitect' //V1.1
import VueRouter from 'vue-router'
Vue.use(BootstrapVue);
Vue.use(VueRouter)
export default {
  name: 'app',
  data: function(){
    return {
      showPage: "homepage"
    }
  },
  components: {
    Homepage,
    Navbar,
    Footer,
    FindArchitect
  },
  //Added for V1.1
  methods : {
    updatePage : function(value) {
      this.showPage = value
    }
  }
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
}

.minSectionHeight{
  min-height: 50vh !important;
}
</style>