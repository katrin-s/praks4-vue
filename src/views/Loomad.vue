<template>
  <div class="">
    <NavBar />
    <Loomad />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import Loomad from '@/components/Loomad.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'loomad',
  components: {
    NavBar,
    Loomad,
    Footer,
  },
};
</script>