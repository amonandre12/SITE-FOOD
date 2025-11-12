<script setup>
import MainCard from './MainCard.vue'

// const openReadmeInEditor = () => fetch('/__open-in-editor?file=README.md')
</script>

<template>
  <div class="image-container">

    <MainCard>
      <img src="@/assets/popsicle.jpg" alt="popsicle-image" />
      <h2>
        Tout ce dont j'ai besoin,<br />
        c'est d'une glace
      </h2>
      <p>
        Le texte Lorem ipsum présente tincidunt <br />
        ipsum lipsum.
      </p>
    </MainCard>

    <MainCard class="salmon-image">
      <img src="@/assets/salmon.jpg" alt="salmon-image" />
      <h2>
        Du saumon pour votre<br />
        peau
      </h2>
      <p>
        Encore une fois, un texte aléatoire au <br />
        texte de Lorem Lorem Lorem Lorem<br />
        ipsum présente tincidunt ipsum Lipsum.
      </p>
    </MainCard>

    <MainCard class="sandwich-image">

      <img src="@/assets/sandwich.jpg" alt="sandwich-image" />
      <h2>
        Le sandwich parfait, un<br />
        vrai classique
      </h2>
      <p>
        Juste un texte aléatoire, le texte de Lorem<br />
        ipsum présente tincidunt ipsum lipsum.
      </p>
      <p>Quoi d'autre?</p>
    </MainCard>

    <MainCard class="croissant-image">
      <img src="@/assets/croissant.jpg" alt="croissant-image" />
      <h2>Le Français</h2>
      <p>
        Lorem lorem lorem lorem ipsum texte<br />
        présent tincidunt ipsum lèvresum.
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
  margin-top: 20px;
}

.image-container img {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
}

@media (min-width: 769px) {
  .image-container {
    display: flex;
    flex-direction: row;
    padding: 70px;
    position: relative;
    bottom: 70px;
  }

  .image-container img {
    width: 350px;
    height: 390px;
  }
  .salmon-image {
    margin-top: 18px;
  }
  .sandwich-image {
    margin-top: 38px;
  }
  .croissant-image {
    margin-bottom: 17px;
  }
}
</style>
