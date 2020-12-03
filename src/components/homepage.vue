<template>
  <div class="homepage">
    <b-container>
      <b-row align-h="center">
    <Introduction/>
    </b-row>
    <div id='grad' >
    <b-row align-h="center">
    <Floorplan/>
    </b-row>
    <b-row align-h="center">
    <Architect/>
    </b-row>
    <b-row align-h="center">
    <Scan/>
    </b-row>
    </div>
    </b-container>
  </div>
</template>

<script>
import Introduction from './introduction.vue'
import Floorplan from './floorplan.vue'
import Architect from './architect.vue'
import Scan from './scan.vue'

export default {
  components: { Introduction, Floorplan, Architect, Scan },
  name: 'Homepage',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
#grad{
  background-image: linear-gradient(white, rgb(209,220,240))
}
</style>
