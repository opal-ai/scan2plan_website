<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/19/2020    Adding Connect Architect functionality
--->

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
import Homepage from './components/Homepage/homepage';
import Navbar from './components/navbar.vue';
import Footer from './components/footer.vue';
import ArchitechtInterface from './components/Architect/architectInterface' //V1.1

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
