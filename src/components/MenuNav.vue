<script setup>
import MainCard from './MainCard.vue'

import { defineEmits } from 'vue';

const emit = defineEmits (['toggle'])

</script>

<template>
  <div class="menu-nav">

    <MainCard class="nav">
      <h2 @click="emit('toggle')">Fermer le menu</h2>
    </MainCard>

    <MainCard class="nav">
      <h2>Nourriture</h2>
    </MainCard>

    <MainCard class="nav">
      <h2>A propos</h2>
    </MainCard>
  </div>
</template>

<style scoped>
.menu-nav {
  border: 1px solid #E2EBF0;
  box-shadow: 0 4px 6px rgba(7, 3, 3, 0.1);
  background-color: #fff;
  padding: 10px;
  z-index: 1000;
  margin-left: -18px;
  padding-bottom: 340px;
  display: flex;
  flex-direction: column;
  gap: 25px;
  width: 510px;
  position: fixed;
  left: 2;
  top: 0;
}
.nav {
  cursor: pointer;
  padding: 6px;
  border-radius: 5px;
}
.nav:hover {
  background-color: #D4D3DC;
}

@media (max-width :769px) {
  .menu-nav {
    width: 310px;
    height: 538px;
  }
.nav {
  position: relative;
  left: 10px;
  padding: 1px;
}
}
</style>
