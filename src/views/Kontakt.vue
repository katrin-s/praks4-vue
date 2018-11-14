<template>
  <div class="">
    <NavBar />
    <Kontakt />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import Kontakt from '@/components/Kontakt.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'kontakt',
  components: {
    NavBar,
    Kontakt,
    Footer,
  },
};
</script>