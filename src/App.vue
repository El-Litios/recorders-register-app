<template>
  <v-app>
    <Navbar />
    <Titulo />
    <Home />
    <router-view />
  </v-app>
</template>

<script>
import Navbar from '@/components/Navbar/Navbar.vue';
import Titulo from '@/components/Titulo/Titulo.vue';
import Home from '@/views/Home.vue';

export default {
  name: 'App',
  components: {
    Titulo, Navbar, Home
  },

  data: () => ({
    //
  }),
};
</script>
