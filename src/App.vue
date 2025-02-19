<template>
  <v-app>
    <Navbar/>
    <v-main>
      <RouterView/>
    </v-main>
  </v-app>
  
 
</template>

<script setup>
//import Home_page from './components/Home_page.vue'
import {RouterView } from 'vue-router';
import Navbar from './components/Navbar.vue';
</script>

