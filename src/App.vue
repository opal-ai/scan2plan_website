<template>
  <div id="app">
    <Navbar/>
    <Homepage />
    <!-- <ScanForm/> -->
    <BottomNavbar/>
  </div>
</template>

<script>
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import Vue from 'vue'
import { BootstrapVue } from 'bootstrap-vue'
import Homepage from './components/homepage.vue'
import Navbar from './components/navbar.vue'
// import ScanForm from './components/scan_form.vue'
import BottomNavbar from './components/bottom_navbar.vue'
// import { library } from '@fortawesome/fontawesome-svg-core'
// import { faUserSecret } from '@fortawesome/free-solid-svg-icons'
// import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

// library.add(faUserSecret)
// Vue.component('font-awesome-icon', FontAwesomeIcon)
// Vue.config.productionTip = false
Vue.use(BootstrapVue)
export default {
  name: 'app',
  components: {
    Homepage,
    Navbar,
    // ScanForm,
    BottomNavbar,
  }
}
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
