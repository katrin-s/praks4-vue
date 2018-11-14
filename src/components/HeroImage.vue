<template>
  <div class="hello">
   <div id="hero-image">
   </div>
  </div>
</template>

<script>
export default {
  name: 'HeroImage',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#hero-image {
    background-image: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.2)), url("https://images.unsplash.com/photo-1518791841217-8f162f1e1131?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=2d7b1bd980752bb3ea0a259f528eae78&auto=format&fit=crop&w=1350&q=80");
    height: 70vh;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    position: relative;
}
@media only screen and (max-width: 1240px) {
    #hero-image {
    display: none;
    }
    }

</style>
