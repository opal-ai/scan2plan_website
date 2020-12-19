<!-- @format -->

<template>
  <div class="homepage">
    <b-container fluid>
      <b-row align-h="center">
        <Introduction />
      </b-row>
      <div id="grad">
        <b-row align-h="center">
          <FloorplanSection />
        </b-row>
        <b-row align-h="center">
          <ArchitectSection @showArchitechtInterface="updateVarForArchitecht"/>
        </b-row>
        <b-row align-h="center">
          <ScanSection />
        </b-row>
      </div>
    </b-container>
  </div>
</template>

<script>
import Introduction from './introduction.vue';
import FloorplanSection from './floorplanSection';
import ArchitectSection from './architectSection.vue';
import ScanSection from './scanSection.vue';

export default {
  components: { Introduction, FloorplanSection, ArchitectSection, ScanSection },
  name: 'Homepage',
  data: function() {
    return {
      showArchitectInterface: false
    }
  },
  props: {},
  methods: {
    updateVarForArchitecht : function(){
      this.showArchitectInterface = true;
      console.log("data passed to homepage")
    }
  }
};
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
#grad {
  background-image: linear-gradient(white, rgb(209, 220, 240));
}
</style>
