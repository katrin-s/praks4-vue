<template>
  <div class="hello">
    <footer>
       <!-- See tee võibolla gridiga -->
       <section class="footer-content">
       <div class="footer-item-1">
           <h2>TOETUSED IGAPÄEVATEGEVUSEKS<br>(RAVI, TOIT, HOOLDUSVAHENDID):</h2>
           <p>Konto: EE10 2200 2210 XXXX XXXX</p>
           <br>
           <h2>VIGASTATUD LOOMADE RAVI:</h2>
           <p>Konto: EE10 2200 2210 XXXX XXXX</p>
           <br>
           <h2>REMONT JA EHITUS:</h2>
           <p>Konto: EE10 2200 2210 XXXX XXXX</p>
           <br>
           <p>Saaja: TARTU KHK LOOMADE VARJUPAIK</p>
           <br>
       </div>
       <div class="footer-item-2">
           <h2>TARTU KHK LOOMADE VARJUPAIK</h2>
           <p>+372 7 361 866<br>
           info@khk.ee<br>
           Kopli 1, 50115 Tartu<br>
           Varjupaika haldab Tartu KHK
           </p>
       </div>
       <div class="footer-item-3">
           <h2>TOETAJAD</h2>
           <img src="https://khk.ee/wp-content/themes/khk/images/KHK-Homepage-1200/logo.png" alt="Tartu Kutsehariduskeskuse logo">
           <img src="https://khk.ee/wp-content/themes/khk/images/KHK-Homepage-1200/logo.png" alt="Tartu Kutsehariduskeskuse logo">
           <img src="https://khk.ee/wp-content/themes/khk/images/KHK-Homepage-1200/logo.png" alt="Tartu Kutsehariduskeskuse logo">
           <img src="https://khk.ee/wp-content/themes/khk/images/KHK-Homepage-1200/logo.png" alt="Tartu Kutsehariduskeskuse logo">
       </div>
       </section>
   </footer>
  </div>
</template>

<script>
export default {
  name: 'Footer',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    footer {
    width: 100%;
    background-color: white;
    min-height: 350px;
    position: relative;
    bottom: 0;
    color: black;
}

.footer-content {
    display: flex;
    width: 89%;
    overflow: hidden;
    margin-left: auto;
    margin-right: auto;
    justify-content: space-between;
    line-height: 170%;
}

div.footer-item-1, div.footer-item-2, div.footer-item-3 {
    padding-right: 20px;
    padding-top: 20px;
    flex-shrink: 0;
    width: 32.5%;
}

footer img {
    width: 160px;
    height: auto;
    padding: 10px;
}

@media only screen and (max-width: 1340px) {

footer img {
    width: 120px;
}
}
@media only screen and (max-width: 1240px) {
    .footer-content {
    flex-direction: column;
    align-items: center;
    text-align: center;
    }
    div.footer-item-1 {
    order: 1;
    padding-bottom: 0;
    width: auto;
    }
    div.footer-item-2 {
    order: 3;
    margin-bottom: 20px;
    width: auto;
    }
    div.footer-item-3 {
    order: 2;
    width: auto;
    }
    }

</style>
