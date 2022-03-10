<template>
  <div>
      <br>
      <h5>REDES SOCIALES</h5>
      <v-row>
          <v-col cols="12" md="6" sm="12">
              <v-text-field label="URL LINKEDIN" required solo></v-text-field>
          </v-col>
          <v-col cols="12" md="6" sm="12">
              <v-text-field label="Usuario de DISCORD" required solo></v-text-field>
          </v-col>
          <v-col cols="12" md="6" sm="12">
              <v-text-field label="URL BEHANCE" solo></v-text-field>
          </v-col>
          <v-col cols="12" md="6" sm="12">
              <v-text-field label="URL GITHUB" solo></v-text-field>
          </v-col>
      </v-row>
      <h5>También puedes incluir otras redes o url personales</h5>
      <v-row>
          <v-col cols="12" md="6" sm="12">
              <v-text-field label="ESCRIBE TU @ INSTAGRAM" required solo></v-text-field>
          </v-col>
          <v-col cols="12" md="6" sm="12">
              <v-text-field label="ESCRIBE TU URL" required solo></v-text-field> 
          </v-col>
      </v-row>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>