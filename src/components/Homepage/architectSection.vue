<!-- @format -->

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
              <b-modal id="loginSignupModal">
                <button class="modalButton" v-on:click="showArchitectLogin">Login as Architect</button>
                <button class="modalButton">Login as Customer</button>
                <button class="modalButton">Sign Up</button>
              </b-modal>
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
      showModal: false,
      showArchitecht: false
    }
  },
  methods: {
    showArchitectLogin : function(){
      this.showArchitecht = true;
      this.$emit("showArchitechtInterface", this.showArchitecht)
    }
  }
};
</script>

<style scoped>
  .modalButton {
    width: 100% 
  }
</style>
