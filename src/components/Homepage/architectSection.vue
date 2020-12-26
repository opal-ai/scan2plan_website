<!-- @format -->
<!--Version History--->
<!--
V1.0    Robert    12/12/2020    Initial Version
V1.1    Aditi     12/19/2020    Added Modal for login on button click
--->

<template>
  <div id="architect">
    <b-container>
      <b-row align-v="center">
        <b-col cols="auto">
          <p style="margin-top:7vh; font-size:2.5rem; font-weight:bolder">FIND AN ARCHITECT</p>
          <p style="font-size:1.5rem; margin-top:2vh">ScanTo3D will help you find the right architect in seconds</p>
          <button
            type="button"
            id="architectButton"
            href="#"
            style="margin-bottom:5vh"
            v-b-modal.loginSignupModal
          >
            Architect Connect
          </button>
          <!--V1.1 changes start-->
              <b-modal id="loginSignupModal">
                <!-- <button class="modalButton" v-on:click="showArchitectLogin">Find an Architect</button>
                <button class="modalButton">Find a project</button> -->
                <h3>Coming soon!</h3>
                <p>Architect Connect will allow you to connect with several architects via our platform. You will be able to see their past projects, ratings etc and chat with them before hiring. 
                  <br> So now you don't have to look all over the internet for a suitable architect. Just browse through our highly skilled partners.
                </p>
              </b-modal>
          <!--V1.1 changes start-->
        </b-col>
        <b-col>
           <b-img fluid-grow :src="require('../../assets/girl.png')" id="architectImage"></b-img>
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

  #architect{
      width:100%
  }

  #architectButton{
    background-color: #044790;
    padding: 7px;
    border-radius: 10px;
    font-size: 0.75rem;
    color:white;
    width: 50%;
    font-size: 1.2rem;
    margin-top: 1vh
  }

  #architectImage{
    border-radius: 20px;
    box-shadow: #808080 5px 5px 10px
  }
</style>
