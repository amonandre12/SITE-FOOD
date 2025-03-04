<script setup>
import ImageContainer from './components/ImageContainer.vue'
import SectionImage from './components/SectionImage.vue'
import NumbersContent from './components/NumbersContent.vue'
import BigImage from './components/BigImage.vue'
import FooterContainer from './components/FooterContainer.vue'
import MenuNav from './components/MenuNav.vue'

import {ref} from "vue";
const showMenu = ref(false) ;

const toggleMenu = () => {
  showMenu.value = !showMenu.value
}
</script>

<template>
  <header>
    <div class="header">
      <box-icon name="menu" @click="toggleMenu"></box-icon>
      <h2>Ma nourriture</h2>
      <h2>Mail</h2>
    </div>
    <Transition name="slide">
    <MenuNav v-if="showMenu" @toggle="toggleMenu"/>
    </Transition>
  </header>

  <main>
    <ImageContainer/>
    <SectionImage />
    <NumbersContent />
    <BigImage />
    <FooterContainer />
  </main>
</template>

<style scoped>
.header {
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-between;
  position: fixed;
  top: 0;
  z-index: 1000;
  width: 100%;
  max-width: 100%;
}

.slide-enter-active, .slide-leave-active {
  transition: transform 0.5s ease-in-out;
}
.slide-enter-from {
  transform: translateX(-100%);
}
.slide-leave-to {
  transform: translateX(-100%);
}
box-icon {
  margin-left: 3px;
  margin-top: 8px;
  cursor: pointer;
}

box-icon:hover {
  background-color: #d4d3dc;
}

h2 {
  margin-right: 16px;
}
@media (min-width :769px) {
  box-icon {
    margin-left: 60px;
  }
  h2 {
    margin-right: 60px;
  }
}
</style>
