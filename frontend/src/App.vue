<template>
    <main class="container pt-4">
      <div>
        <router-link :to="{name: 'Main Page'}">Main Page</router-link>
        |
        <router-link :to="{name: 'Articles List'}">Articles</router-link>
        |
        <router-link :to="{name: 'Register'}">Register</router-link>
        |
        <router-link :to="{name: 'Login Page'}">Login</router-link>
        |
        <router-link :to="{name: 'Profile Page'}">My Profile</router-link>
      </div>
      <RouterView class="flex-shrink-0" />
    </main>
  </template>
  
  <script lang="ts">
  import { defineComponent } from "vue";
  import { RouterView } from "vue-router";
  
  export default defineComponent({
      components: { RouterView },
  });
  </script>
  
  <style scoped>
  </style>
  
