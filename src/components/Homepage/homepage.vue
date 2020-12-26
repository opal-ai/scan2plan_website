<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/19/2020    Toggle interface based on selection
--->

<template>
  <div class="homepage">
        <Introduction />
      <div id="grad">
        <b-row align-h="center" align-v="center" class = "minSectionHeight">
          <FloorplanSection />
        </b-row>
        <b-row align-h="center"  align-v="center" class = "minSectionHeight">
          <ArchitectSection @showInterface="updateInterface"/> <!--V1.1 change-->
        </b-row>
        <b-row align-h="center" align-v="center" class = "minSectionHeight">
          <ScanSection />
        </b-row>
      </div>
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
  background-image: linear-gradient(rgb(8 71 144 / 44%), rgb(242 247 253))
}


</style>
