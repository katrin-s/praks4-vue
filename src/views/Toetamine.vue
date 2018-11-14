<template>
  <div class="">
    <NavBar />
    <Toetamine />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import Toetamine from '@/components/Toetamine.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'toetamine',
  components: {
    NavBar,
    Toetamine,
    Footer,
  },
};
</script>
