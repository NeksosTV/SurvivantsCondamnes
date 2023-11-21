<template>
  <nav class="navigation p-4">    <!-- changer la couleur de gb du menu -->
    <div class="flex items-center justify-between">
      <div class="flex items-center">
         <span class="text-white text-xl font-semibold mr-4"></span> <!--mettre un titre ici comme logo si on le souhaite -->
      </div>
      <div class="md:hidden">
        <button
          @click="isOpen = !isOpen"
          type="button"
          class="text-gray-500 hover:text-white focus:outline-none focus:text-white"
        >
          <svg
            class="h-6 w-6 fill-current"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <!-- Icône hamburger -->
          </svg>
        </button>
      </div>
      <div
        :class="{
          'hidden': !isOpen,
          'md:flex md:items-center w-full md:w-auto': true
        }"
        class="mt-4 md:mt-0"
      >
        <ul class="md:flex space-y-4 md:space-y-0 md:space-x-4">
          <li>
            <NuxtLink to="/" class="block text-white hover:text-gray-300">Accueil</NuxtLink>
          </li>
          <li>
            <NuxtLink to="/about" class="block text-white hover:text-gray-300">À propos</NuxtLink>
          </li>
          <!-- <li>
            <NuxtLink to="#" class="block text-white hover:text-gray-300">Contact</NuxtLink>
          </li> -->
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      isOpen: false,
    };
  },
};
</script>


<style>

</style>