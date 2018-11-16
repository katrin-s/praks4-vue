<template>
  <div class="">
  <section class="kontaktid">
      <div class="kontakt-item-1">
       <h2>kontakt</h2>
       <p>Meiega saab ühendust võtta ööpäevaringselt telefonil +372 7 361 866<br>
Kohaletulekust palume võimaluse korral ette teatada!<br>
Asume aadressil Kopli 1, 50115 Tartu.<br>Maja kõrval on 5 parkimiskohta.<br>
Meie juurde sõidavad bussid nr 4, 9, 11, 12, 13 ja 19. <br>Väljuda tuleb Alasi peatuses ja tulla üle Võru tänava.<br>Busside sõiduplaanid leiad <a href="http://tartu.peatus.ee" target="_blank" class="outer-link"><strong>SIIT</strong></a><br>
E-kirjadele vastame esimesel võimalusel, hiljemalt 3 tööpäeva jooksul: info@khk.ee
</p>
       </div>
       <div class="maps">
       <iframe class="iframe" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2093.6054081752854!2d26.71191935169235!3d58.34945819614565!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46eb3747db90ed05%3A0x387b666bb555e743!2sKopli+1%2C+50115+Tartu!5e0!3m2!1sen!2see!4v1540967788421" width="100%" height="100%" style="border:0" allowfullscreen></iframe>
       </div>
   </section>
  </div>
</template>

<script>
export default {
  name: 'Kontakt',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.kontaktid {
    display: flex;
    width: 89%;
    margin: 120px auto 0 auto;
    flex-direction: column;
    text-align: center;
}

.kontakt-item-1 {
    margin: auto;
    margin-top: auto;
    margin-bottom: auto;
    line-height: 170%;
    }
   .maps {
    margin: auto;
    padding-top: 10px;
    width: 60vw;
    height: 40vh;
    margin-bottom: 20px;
}
</style>
