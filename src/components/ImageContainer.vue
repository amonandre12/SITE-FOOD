<script setup>
import MainCard from './MainCard.vue'
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="image-container">

    <MainCard class="sandwich-image">
      <img src="@/assets/sandwich.jpg" alt="sandwich-image" />
      <h2>
        Le sandwich parfait, un <br />
        véritable classique de <br />
        New York
      </h2>
      <p>
        Juste un texte aléatoire, le texte de Lorem<br />
        ipsum présente tincidunt ipsum lipsum.
      </p>
    </MainCard>

    <MainCard class="steak-image">
      <img src="@/assets/steak.jpg" alt="steak-image" />
      <h2>
        Laissez-moi vous parler<br />
        de ce steak
      </h2>
      <p>
        Encore une fois, un texte aléatoire au <br />
        texte de Lorem<br />
        ipsum présente tincidunt ipsum lipsum.
      </p>
    </MainCard>

    <MainCard class="cherries-image">

      <img src="@/assets/cherries.jpg" alt="cherries-image" />
      <h2>Cerises, interrompues</h2>
      <p>
        Le texte Lorem ipsum présente tincidunt <br />
        ipsum lipsum.
      </p>
      <p>Quoi d'autre?</p>

    </MainCard>

    <MainCard class="wine-image">
      <img src="@/assets/wine.jpg" alt="wine-image" />
      <h2>
        Encore une fois, du vin <br />
        robuste et des pâtes aux <br />
        légumes
      </h2>
      <p>
        Le texte Lorem ipsum présente tincidunt <br />
        ipsum lipsum.
      </p>
    </MainCard>
  </div>
</template>

<style scoped>
.image-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
  padding: 20px;
  text-align: center;
  margin-top: 60px;
}

.image-container img {
  max-width: 100%;
  height: auto;
  border-radius: 2px;
}

@media (min-width: 769px) {
  .image-container {
    display: flex;
    flex-direction: row;
    padding: 70px;
  }

  .image-container img {
    width: 350px;
    height: 390px;
  }
  .cherries-image {
    margin-top:6px;
  }
  .steak-image {
    margin-top:17px;
  }
  .wine-image {
    margin-top:27px;
  }
  .sandwich-image {
    position: relative;
    top: 12px;
  }
}
</style>
