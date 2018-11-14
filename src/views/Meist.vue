<template>
  <div class="">
    <NavBar />
    <Meist />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import Meist from '@/components/Meist.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'meist',
  components: {
    NavBar,
    Meist,
    Footer,
  },
};
</script>