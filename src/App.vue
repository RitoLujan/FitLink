<template>
  <FitLinkMenu/>
</template>

<script>
import FitLinkMenu from './components/FitLinkMenu.vue'
import 'bootstrap/dist/css/bootstrap.min.css';
import 'jquery';
import 'popper.js';
import 'bootstrap';

export default {
  name: 'App',
  components: {
    FitLinkMenu
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
}
</style>
