<template>
  <v-toolbar color="white" flat class="NabvarTools">
      <v-toolbar-title>
        <v-img
        max-height="200"
        max-width="200"
        src="../../assets/logoRecoders.png"
        ></v-img>
      </v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn elevation="0" x-large plain>
        Recoders
      </v-btn>

      <v-btn elevation="0" x-large plain>
        Directorio
      </v-btn>

      <v-btn elevation="0" x-large plain>
        Contacto
      </v-btn>

    </v-toolbar>
</template>

<script>
export default {
  
}
</script>

<style scoped>
    @import 'Navbar.css';
</style>