<template>
  <div class="home">
    <NavBar />
    <HeroImage />
    <FrontPage />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import HeroImage from '@/components/HeroImage.vue';
import FrontPage from '@/components/FrontPage.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'home',
  components: {
    NavBar,
    HeroImage,
    FrontPage,
    Footer,
  },
};
</script>
