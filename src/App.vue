<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-img alt="Mailbox Logo" class="shrink mr-2" contain src="./assets/images/mailbox-white.png" transition="scale-transition" width="40"/>
        <h1>PQRS</h1>
      </div>

      <v-spacer></v-spacer>

      <router-link to="/registro">
        <v-btn text>Registro</v-btn>
      </router-link>
      
    </v-app-bar>

    <v-main>
      <router-view/>
      <!-- <PQRSAdmin/> -->
    </v-main>
    
  </v-app>
</template>

<script>
// import PQRSAdmin from './views/PQRSAdmin.vue';

export default {
  name: 'App',

  components: {
    // PQRSAdmin
  },

  data: () => ({
    //
  }),
};
</script>

<style >
  @import './assets/scss/style.css';
</style>

