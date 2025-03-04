<script setup>
import MainCard from './MainCard.vue'
</script>

<template>
  <MainCard class="big-image">
    <h2>À propos de moi, l'homme de la nourriture</h2>

    <MainCard>
      <img src="@/assets/chef.jpg" alt="chef-image" class="image">
    </MainCard>

    <MainCard>
      <h3>Je suis qui je suis !</h3>
      <em>Avec passion pour la vraie et bonne cuisine</em>
    </MainCard>

    <MainCard class="paragraph">
      <p>
        Juste moi, moi et moi, explorant l'univers de l'inconnu. J'ai un cœur d'amour et un intérêt pour le blog Lorem ipsum et Mauris Neque Quam. Je veux partager mon monde<br>
        avec toi. Praesent tincidunt sed tellus ut rutrum. Sed vitae justo condimentum, porta lectus vitae, ultricies congue gravida diam non fringilla. Praesent tincidunt sed tellus ut<br>
        rutrum. Sed vitae justo condimentum, porta lectus vitae, ultricies congue gravida diam non fringilla.
      </p>
    </MainCard>

  </MainCard>
  <hr>
</template>

<style scoped>
.big-image {
  padding: 20px;
  text-align: center;
  max-width: 100%;
  margin-top: 120px;
}

.big-image img {
  margin-top: 50px;
}

hr {
  position: relative;
  top: 2px;
}
.image {
  max-width: 100%;
  height: auto;
  border-radius: 10px;
  display: block;
  margin: 0 auto;
}


h2 {
  font-size: clamp(1.5rem, 1.8vw, 2.5rem);
  font-weight: bold;
}
.paragraph {
  margin-top: 10px;
}
h3 {
  font-size: clamp(1.2rem, 1.5vw, 2rem);
  font-weight: bold;
}

p {
  font-size: clamp(1rem, 1vw, 1.2rem);
  max-width: 100%;
  margin: 0 auto;
  line-height: 1.6;
  padding: 10px;
}
@media (min-width: 769px)  {
  .paragraph {
    text-align: center;
  }
  .big-image {
    margin-top: 220px;
  }
}
</style>
