<template>
  <div class="toetamine">
    <section class="kuidas">
     <h2>KUIDAS MEID TOETADA?</h2>
     <div class="toetused">
      <div class="rahaline">
         <h2>RAHALINE TOETUS</h2>
         <p>Varjupaiga igapäevast tegevust saab toetada meie tegevuskontole:
<br><br>
TARTU KHK LOOMADE VARJUPAIK<br><br>
IBAN: EE1022002210XXXXXXXX
<br><br>
Igapäevane tegevus tähendab loomade toitu ja igapäevaseid raviprotseduure, samuti kastreerimist/steriliseerimist. 
<br><br>
Varjupaika saabuvate vigastatud loomade abi saab toetada meie kiirabikontole:
<br><br>
TARTU KHK LOOMADE VARJUPAIK<br><br>
IBAN: EE1022002210XXXXXXXX
<br><br>
Operatiivne ravi tähendab nn traumapatsiente (avariilised loomad, teiste loomade rünnakute ohvrid jms), kus on vaja looma kiirelt aidata. Selle konto raha kasutatakse ainult vältimatu abi jaoks.
<br><br>
Varjupaiga arendus- ja ehitustegevust saab toetada meie ehituskontole:
<br><br>
TARTU KHK LOOMADE VARJUPAIK<br><br>
IBAN: EE1022002210XXXXXXXX
<br><br>
Raha läheb varjupaigas olevate loomade hoiuolukorra parandamiseks.</p>
          
      </div>
      <div class="materiaalne">
         <h2>MATERIAALNE TOETUS</h2>
         <P>Varjupaik võtab alati vastu alljärgnevaid esemelisi annetusi loomadele:
         <br>
         <br>
         kassi ja koera kuivtoit
         <br>
         <br>
         kassi ja koera konservid
         <br>
         <br>
         kassiliiv
         <br>
         <br>
         loomadele sobilikud mänguasjad (pallid, nutsud, koeraköied, ronimis- ja küüneteritamisalused)
         <br>
         <br>
         kaela- ja jalutusrihmad (parimad on presendist), ketikarabiinid ja -pööritsad
         <br>
         <br>
         aluspanu- ja pesamaterjal (vati-, baika, fliis- ja villatekid)
         <br>
         <br>
         froteevannilinasid ja froteekäterätikud - loomade kuivatamiseks, allapanuks
         <br>
         <br>
         erinevates mõõtudes transpordiboksid ja näitusepuurid
         <br>
         <br>
         puhastusvahendid (desinfitseerivate omadustega kontsentraadid, üldpuhastusvahendid, pesupulber, nõudepesuvahendid)
         <br>
         <br>
         koristusvahendid (harjad, mopid, nuustikud, kühvlid ja ämbrid) 
         </P>
          
      </div>
      <div class="vabatahtlik">
         <h2>VABATAHTLIKUNA ABISTAMINE</h2>
         <p>Kui soovid tulla vabatahtlikuks, anna meile oma soovist teada vähemalt üks päev ette.
         <br>
         <br>
Varjupaigas tehtavate tööde loetelu:
<br>
         <br>
Heakorratööd (rohimine, riisumine, trimmeriga niitmine, lumekoristus)<br>
         <br>
Küttepuude ladumine<br>
         <br>
Ehitus- ja remonditööd (kuutide parandamine, värvimine jms)<br>
         <br>
Üldpuhastustööd (seinte, akende ja põrandate pesemine)<br>
         <br>
Loomade hoiupaikade puhastamine juhendamisel (kuutide ja nende ümbrus või kassipuurid)<br>
         <br>
Loomade hooldamine juhendamisel (kammimine)<br>
         <br>
Loomadele vee jagamine (põhiliselt koerad)<br>
         <br>
Koerte jalutamine territooriumil koos hoiupaiga puhastamisega (ehk kuudi ümbrus) - kogenud vabatahtlikele </p>
          
      </div>
      </div>
       <div>
           <button id="go-up">&#94; &Uuml;LES</button>
       </div>
       
   </section>
  </div>
</template>

<script>
export default {
  name: 'toetamine',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    
.kuidas {
    width: 89%;
    margin: 120px auto 0 auto;
    text-align: center;
}

.toetused {
    display: flex;
    text-align: left;
    margin: 0 auto;
}

.materiaalne, .rahaline, .vabatahtlik {
    padding-right: 20px;
    line-height: 140%;
    flex-shrink: 0;
    width: 32.5%;
}
    
    .rahaline>p {
    padding-bottom: 10px;
    }

.kuidas>h2 {
    padding-bottom: 40px;
}

@media only screen and (max-width: 1240px) {
    .toetused {
    flex-direction: column;
    text-align: center;
}
    .materiaalne, .rahaline, .vabatahtlik {
    padding-right: 0;
    line-height: 170%;
    width: 100%;
    margin-bottom: 20px;
}
}

</style>
