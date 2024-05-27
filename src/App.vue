<script setup>
import NavMenu from './components/parts/NavMenu.vue';
</script>

<template>
  <NavMenu/>
  <div class="py-24">
    <router-view></router-view>
  </div>
  
</template>

<style scoped>
h1{
  color: black;
}
</style>