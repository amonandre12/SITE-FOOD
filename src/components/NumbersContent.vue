<script setup>
import MainCard from './MainCard.vue'
</script>

<template>
<MainCard class="numbers-content">

  <MainCard>
    <box-icon name='chevrons-left'></box-icon>
  </MainCard>

  <MainCard>
    <a href="#" class="number-one">1</a>
  </MainCard>

  <MainCard>
    <a href="#" class="link-2">2</a>
  </MainCard>

  <MainCard>
    <a href="#" class="link-3">3</a>
  </MainCard>

  <MainCard>
    <a href="#" class="link-4">4</a>
  </MainCard>

  <MainCard>
    <box-icon name='chevrons-right' class="chevrons-right"></box-icon>
  </MainCard>
</MainCard>
<hr>
</template>

<style scoped>
.numbers-content {
  display: flex;
  flex-direction: row;
  gap: 30px;
  text-align: center;
  justify-content: center;
  position: relative;
  top: 30px;
}

.link-2 {
  position:relative;
  top:1px;
}


.link-3 {
  position:relative;
  top:1px;
}

.link-4 {
  position:relative;
  top:2px;
}

hr {
  position: relative;
  top: 80px;
}
a {
  text-decoration: none;
  color: black;
  padding: 7px 10px 7px 10px;
}

a:hover {
  background-color: black;
  color: white;
}
.number-one {
  background-color: black;
  color: white;
  padding: 7px 10px 7px 10px;
}

box-icon {
  cursor: pointer;
}

@media (min-width: 769px) {

hr {
  position: relative;
  top: 150px;
  height: 6px;
}
}
</style>
