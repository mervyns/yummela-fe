<template>
  <header class="bg-gray-900 sm:flex sm:justify-between sm:items-center sm:px-4 sm:py-3">
    <div class="flex items-center justify-between px-4 py-3 sm:p-0">
      <a href="#" class="block px-2 py-1 text-white font-semibold rounded hover:bg-gray-800">yummela</a>
    </div>
    <nav class="px-2 pt-2 pb-4 sm:flex sm:p-0">
      <a href="#" class="mt-1 block px-2 py-1 text-white font-semibold rounded hover:bg-gray-800 sm:mt-0 sm:ml-2">Explore Eats</a>
      <a href="#" class="block px-2 py-1 text-white font-semibold rounded hover:bg-gray-800">List your eats</a>
      <a href="#" class="mt-1 block px-2 py-1 text-white font-semibold rounded hover:bg-gray-800 sm:mt-0 sm:ml-2">Sign Up / Login</a>
      <button @click="showAuthModal" type="button" class="block text-white hover:text-white focus:text-white focus:outline-none">
          Sign Up / Login
      </button>
    </nav>
  </header>
</template>
<script>
import { mapMutations } from 'vuex'

export default {
  data() {
    return {
      navbarOpen: false,
    };
  },
  methods: {
    ...mapMutations({
      showAuthModal: "showAuthModal",
      hideAuthModal: "hideAuthModal"
    }),
    setNavbarOpen: function () {
      this.navbarOpen = !this.navbarOpen;
    },
  },
};
</script>