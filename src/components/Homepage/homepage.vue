<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/19/2020    Toggle interface based on selection
--->

<template>
  <div class="homepage">
    <b-container fluid>
     
        <Introduction />
      
      <div id="grad">
        <b-row align-h="center" class = "minSectionHeight">
          <FloorplanSection />
        </b-row>
        <b-row align-h="center" class = "minSectionHeight">
          <ArchitectSection @showInterface="updateInterface"/> <!--V1.1 change-->
        </b-row>
        <b-row align-h="center" class = "minSectionHeight">
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
      showInterface: ""
    }
  },
  props: {},
  //V1.1
  methods: {
    updateInterface : function(value){
      this.showInterface = value;
      this.$emit("showInterface", this.showInterface)
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
