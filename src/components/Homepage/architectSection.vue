<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/19/2020    Added Modal for login on button click
--->

<template>
  <div id="architect">
    <b-container>
      <b-row>
        <b-col cols="auto">
          <h1 style="margin-top:7vh">FIND AN ARCHITECT</h1>
          <h4>Scan2plan helps you find the right architect in seconds</h4>
          <button
            type="button"
            class="btn btn-primary"
            href="#"
            style="margin-bottom:5vh"
            v-b-modal.loginSignupModal
          >
            Architect Connect
          </button>
          <!--V1.1 changes start-->
              <b-modal id="loginSignupModal">
                <button class="modalButton" v-on:click="showArchitectLogin">Find an Architect</button>
                <button class="modalButton">Find a project</button>
              </b-modal>
          <!--V1.1 changes start-->
        </b-col>
        <b-col>
          <img src="../../assets/girl.png" width="300vw" height="200vw" />
        </b-col>
      </b-row>
    </b-container>
    <!-- <router-view/> -->
  </div>
</template>

<script>
export default {
  name: 'ArchitectSection',
  components: {},
  data: function() {
    return {
      showArchitecht: ""
    }
  },
  //V1.1
  methods: {
    showArchitectLogin : function(){
      this.showArchitecht = "architect";
      this.$emit("showInterface", this.showArchitecht)
    }
  }
};
</script>

<style scoped>
  .modalButton {
    width: 100% 
  }
</style>
