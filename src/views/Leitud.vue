<template>
  <div class="">
    <NavBar />
    <Leitud />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import Leitud from '@/components/Leitud.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'leitud',
  components: {
    NavBar,
    Leitud,
    Footer,
  },
};
</script>