<template>
  <div id="app" class="d-flex flex-column h-100">
    <nav-bar />
    <div class="container flex-grow-1">
      <error />
      <div class="mt-5">
        <router-view />
      </div>
    </div>
    <footer class="bg-light text-center p-3">
      <div class="logo"></div>
      <p>
        
        <a :href="'mailto:guirchounmelvin@gmail.com'">Nous contacter</a>
      </p>
    </footer>
  </div>
  
</template>

<script lang="ts">
import NavBar from "./components/NavBar.vue";
import Error from "./components/Error.vue";
import PaginationBar from "./components/PaginationBar.vue";

export default {
  components: {
    NavBar,
    Error
  }
};
</script>
