<!-- @format -->

<template>
  <div id="app">
    <Navbar />
    <Homepage />
    <Footer />
    <ArchitechtInterface v-if="showArchitect"/>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css';
import 'bootstrap-vue/dist/bootstrap-vue.css';
import Vue from 'vue';
import { BootstrapVue } from 'bootstrap-vue';
import Homepage from './components/homepage.vue';
import Navbar from './components/navbar.vue';
import Footer from './components/footer.vue';
import ArchitechtInterface from './components/architectInterface'
// import $ from 'jquery';
// import { library } from '@fortawesome/fontawesome-svg-core'
// import { faUserSecret } from '@fortawesome/free-solid-svg-icons'
// import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

// library.add(faUserSecret)
// Vue.component('font-awesome-icon', FontAwesomeIcon)
// Vue.config.productionTip = false
// import Vue from 'vue';
//import VueRouter from 'vue-router';

//Vue.use(VueRouter);
Vue.use(BootstrapVue);
export default {
  name: 'app',
  data: function(){
    return {
      showArchitect: false
    }
  },
  components: {
    Homepage,
    Navbar,
    Footer,
    ArchitechtInterface
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
