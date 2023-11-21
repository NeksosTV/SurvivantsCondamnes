<script setup>
import Logo from '../public/img/LogoSC3.png'; // Remplacez le chemin par le chemin de votre logo


</script>

<template>
  <header class=" text-slate-900">
    <div class="wrapper p-6 text-center flex flex-col md:flex-row md:items-center">
      <div class="logo-container md:absolute md:top-0 md:left-0 md:p-10">
        <img class="logo" :src="Logo" alt="Les Survivants Condamnés">
      </div>
      <h1 class="text-4xl md:text-2xl font-bold py-4 md:pl-5 title"></h1>
      <Navigation   :isLoggedIn="isLoggedIn" @logout="logout" />
    </div>
  </header>

</template>

<style scoped>

.title{
  margin-left: 50%;
  text-align: center;
}
.logo-container {
  position: absolute;
  top: 0;
  left: 0;
  padding: 10px;
}

.logo {
  height: 80px; /* Ajustez la hauteur du logo (taille) */
}

@media (max-width: 768px) {
  /* .wrapper {
    flex-direction: column;s
    align-items: center;
  } */

  .logo-container {
    position: relative;
    top: initial;
    left: initial;
    padding: 0;
    margin-bottom: 10px;
  }

  .logo {
    height: 60px; /* Ajustez la hauteur du logo pour les écrans plus petits */
  }

  .text-4xl {
    font-size: 3rem; /* Ajustez la taille du titre pour les écrans plus petits */
  }
}
</style>