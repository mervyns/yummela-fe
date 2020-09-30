<template>
  <div>
    <navbar />
    <main>
      <section class="relative w-full h-full py-40 min-h-screen">
        <router-view />
        <home />
        <footer-small absolute />
      </section>
    </main>
  </div>
</template>
<script>
import Navbar from "@/components/Navbar/Navbar.vue";
import FooterSmall from "@/components/Footers/FooterSmall.vue";
import Home from '@/views/Home.vue';

export default {
  components: {
    Navbar,
    Home,
    FooterSmall,
  },
};
</script>