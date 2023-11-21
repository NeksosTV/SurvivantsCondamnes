<template>
<main>

  <div class="banner">
    <h1 class="text-center title">Les Survivants Condamnés</h1>
    <img class="logo" :src="Logo" alt="Les Survivants Condamnés">

  </div>

  <div class="para">
      <p>Bienvenue Chez Les Survivants Condamnés  ! Nous sommes une communauté DayZ  à croissance rapide, immersive et sans drame. Nous avons une équipe dédiée pour répondre à tous les besoins impliquant des infractions aux règles ou toute aide aux joueurs ! , dans un monde de survie ! Avez-vous ce qu'il faut pour survivre ?!</p>
    </div>
</main>


</template>

<script setup>
import Logo from '../public/img/DayzIngames.png'; // Remplacez le chemin par le chemin de votre logo
</script>

<style scoped>
/* Styles spécifiques au composant */

.banner {
  text-align: center;
  height: 350px;
  position: relative;
  overflow: hidden;
}

.title {
  font-size: 2.55em;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 1;
  color: red;
  font-family: 'Anton', cursive;
}

.logo {
  width: 100%;
  height: 100%;
  object-fit: cover;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 0;
}

.para {
  position: absolute;
  left: 50%; /* Centrer le paragraphe horizontalement */
  transform: translateX(-50%);
  color: aliceblue;
  padding: 20px;
  text-align: center;
  width: 80%;
  font-family: 'Anton', cursive;
}
</style>
