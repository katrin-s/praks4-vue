<template>
  <div class="">
  <section class="meist">
       <h2>MEIST</h2>
       <p>2018. aasta novembris möödub 20 aastat päevast, mil avati Tartu KHK Loomade Varjupaik. Alates sellest ajast on siin käinud igapäevane töö ning meieni on jõudnud paljud Tartu linna ja Lõuna-Eesti kassid ja koerad.

20 aasta jooksul on meie juurest uue kodu leidnud üle 1000 looma.

Kogu igapäevane töö ja loomade ravi toimub ainult tänu headele annetajatele ja toetajatele. 
     <br><br>Suur aitäh!</p>
      <img src="https://images.unsplash.com/photo-1534750554350-5d579939db38?ixlib=rb-0.3.5&s=569d671234a4d9fa951b34de681bd903&auto=format&fit=crop&w=1350&q=80" alt="Team of happy volunteers">
   </section>
  
  </div>
</template>

<script>
export default {
  name: 'Meist',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .meist {
    margin: 120px auto 0 auto;
    display: flex;
    width: 89%;
    flex-direction: column;
    text-align: center;
}

.meist>p {
    padding-left: 20%;
    padding-right: 20%;
    line-height: 170%;
}

.meist>img {
    width: 70vw;
    height: auto;
    margin: auto;
    padding-top: 10px;
    margin-bottom: 20px;
}
@media only screen and (max-width: 1240px) {
    
.meist>p {
    padding-left: 5%;
    padding-right: 5%;
}
    }

</style>