<script setup>
import FooterCard from './FooterCard.vue'
</script>

<template>
  <div class="footer-container">

    <FooterCard class="footer-section">
      <template #title>PIED DE PAGE</template>
      <p class="section-para">
        Praesent tincidunt sed tellus ut rutrum. Sed vitae justo <br>
        condimentum, porta lectus vitae, ultricies congue<br>
        gravida diam non fringilla.
      </p>
      <p class="footer-credit">Propulsé par w3.css</p>
    </FooterCard>


    <FooterCard class="footer-blog">
      <template #title>ARTICLES DE BLOG</template> <br/>
      <div class="blog">
        <img src="@/assets/workshop.jpg" alt="workshop-image"><br>
        <p class="blog-paragraph">Bonjour,<br>
          mais tu es toujours là.
        </p>
      </div>
      <hr>
      <div class="blog-item">
        <img src="@/assets/gondol.jpg" alt="gondol-image">
        <p class="paragraph">C'est<br>
          plutôt teint, mais
      </p>
      </div>
    </FooterCard>


    <FooterCard class="footer-section">
      <template #title>ÉTIQUETTES POPULAIRES</template>
      <div class="tags">
        <img src="@/assets/tableau.jpg" alt="tableau-image">
      </div>
    </FooterCard>
  </div>
</template>

<style scoped>
.footer-container {
  padding: 20px;
  display: flex;
  flex-direction: column;
  gap:40px;
  margin-top: 10%;
}

.footer-credit {
  position: relative;
  left: 2px;
  margin-bottom: 25px;
  font-size: 0.9rem;
  opacity: 0.8;
}
.footer-section {
  max-width: 600px;
  margin-bottom: 20px;
}

.footer-blog {
  max-width: 600px;
  margin-bottom: 20px;
}

.blog {
 display: flex;
 cursor: pointer;
}

.blog:hover {
  background-color: #D4D3DC;
}

.blog-item {
  display: flex;
  cursor: pointer;
  margin-top: 30px;
}

hr {
  margin-top: 30px;
}

.blog-item:hover {
  background-color: #D4D3DC;
}

.blog-paragraph {
  position: relative;
  right: 50px;
}
.paragraph  {
  position: relative;
  right: 65px;
}
.blog img {
  width: 60px;
  height: auto;
  border-radius: 5px;
}
.blog-item img
 {
  width: 60px;
  height: auto;
  border-radius: 5px;
}

.tags img  {
  max-width: 100%;
  height: auto;
  border-radius: 5px;
}

p {
  max-width: 500px;
  margin: 5px auto;
}

@media (min-width: 768px) {
  .footer-container {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
  }

  .tags img  {
    width: 340px;
    margin-top: 40px;
  }

.footer-blog {
  position: relative;
  left:100px;
}
  .blog-item img {
    width: 50px;
    height:50px;
  }
  .section-para {
    position: absolute;
    left: 109px;
    margin-top: 40px;
  }
  .footer-credit {
    position: relative;
    top: 115px;
  }
.blog img {
  width: 50px;
  height: 50px;
  border-radius: 5px;
}
.blog-paragraph {
  margin-left: 76px;
}
.paragraph {
  margin-left: 90px;
}

.blog-item {
  display: flex;
  cursor: pointer;
  margin-bottom: 70px;
}
}
</style>
