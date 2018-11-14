<template>
  <div class="leitud">
    <section class="kuulutused">
      <div class="kuulutus">
         <h2>kuulutuse lisamine</h2>
          <p>Vaatame teie saadetud kuulutuse esimesel võimalusel läbi ning paneme lehele üles.</p>
          <div class="kuulutuse-vorm">
              <form>
                  <h2 id="vormi-pealkiri">lisa kuulutus</h2>
                  <select name = "dropdown">
                      <option value = "Kadunud" selected>Kadunud</option>
                      <option value = "Leitud">Leitud</option>
                  </select>
              </form>
              <form>
                  <select name = "dropdown">
                      <option value = "Kass" selected>Kass</option>
                      <option value = "Koer">Koer</option>
                  </select>
              </form>
              <form >
                  <input type = "text" name = "Nimi" placeholder="Nimi ja värv/tõug">
              </form>
              <form action="">
                  <input type="date" name="Date">
              </form>
              <form>
                  <textarea rows = "5" cols = "42" name = "Kirjeldus" placeholder="Looma pikem kirjeldus ja muu oluline info.">
                  </textarea>
              </form>
              <form>
                  <input type = "file" name = "Upload" accept = "image/*">
              </form>
              <form >
                  <input type = "text" name = "Nimi" placeholder="Teie meiliaadress">
              </form>
              <form >
                  <input type = "text" name = "Nimi" placeholder="Teie telefoninumber">
              </form>
              <input class="saada" type="submit" value="Saada">
          </div>
      </div>
      <div class="lisatud">
      <div class="filter">
         <h2>kadunud/leitud loomad</h2>
          <button type="button">KASSID</button>
          <button type="button">KOERAD</button>
      </div>
      <div class="leitud-grid">
          <div class="loom">
              <div class="info">
                  <h2><b>leitud: </b>must kass kesklinnast
                      <p>
                          KUUPÄEV: 12.12.2019
                          <br>
                          KONTAKT: +372 55 11 22 33
                          <br>
                          emailiaadress@gmail.com  
                      </p></h2>
              </div>
          </div>
          <div class="loom">
              <div class="info">
                  <h2><b>leitud: </b>must kass kesklinnast
                      <p>
                          KUUPÄEV: 12.12.2019
                          <br>
                          KONTAKT: +372 55 11 22 33
                          <br>
                          emailiaadress@gmail.com  
                      </p></h2>
              </div>
          </div>
          <div class="loom">
              <div class="info">
                  <h2><b>leitud: </b>must kass kesklinnast
                      <p>
                          KUUPÄEV: 12.12.2019
                          <br>
                          KONTAKT: +372 55 11 22 33
                          <br>
                          emailiaadress@gmail.com  
                      </p></h2>
              </div>
          </div>
          <div class="loom">
              <div class="info">
                  <h2><b>leitud: </b>must kass kesklinnast
                      <p>
                          KUUPÄEV: 12.12.2019
                          <br>
                          KONTAKT: +372 55 11 22 33
                          <br>
                          emailiaadress@gmail.com  
                      </p></h2>
              </div>
          </div>
          <div class="loom">
          <div class="info">
              <h2><b>leitud: </b>must kass kesklinnast
                  <p>
                      KUUPÄEV: 12.12.2019
                      <br>
                      KONTAKT: +372 55 11 22 33
                      <br>
                      emailiaadress@gmail.com  
                  </p></h2>
          </div>
          </div>
          <div class="loom">
              <div class="info">
                  <h2><b>leitud: </b>must kass kesklinnast
                      <p>
                          KUUPÄEV: 12.12.2019
                          <br>
                          KONTAKT: +372 55 11 22 33
                          <br>
                          emailiaadress@gmail.com  
                      </p></h2>
              </div>
          </div>
          <div class="loom">
              <div class="info">
                  <h2><b>leitud: </b>must kass kesklinnast
                      <p>
                          KUUPÄEV: 12.12.2019
                          <br>
                          KONTAKT: +372 55 11 22 33
                          <br>
                          emailiaadress@gmail.com  
                      </p></h2>
              </div>
          </div>
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
  name: 'Leitud',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .kuulutused {
    margin: 120px auto 0 auto;
    width: 89%;
    display: flex;
    justify-content: space-between;
}
    
    .kuulutus {
        width: 320px;
        margin-right: 40px;
    }
    
    .kuulutus>h2, .filter>h2 {
        padding-bottom: 10px;
        padding-top: 10px;
    }
    
    textarea {
        resize: none;
        height: 140px;
    }
    
    form, select, input, textarea {
        width: 240px;
        margin: 4px auto;
        position: relative; 
    }
    
    .kuulutuse-vorm {
        width: 360px;
        height: 520px;
        background-color: #98E4E4;
        display: flex;
        align-content: center;
        flex-direction: column;
        margin: 20px 0;
    }
    
    .saada {
        padding: 8px;
        background-color: #B7FFFF;
        border-radius: 30px;
        width: 100px;
        text-transform: uppercase;
        font-size: 18px;
        font-weight: 700;
    }
    
    #vormi-pealkiri {
        margin: 8px 40px;
    }
    
    .leitud-grid {
        display: flex;
        flex-wrap: wrap;
    }

    .loom {
        background: url(https://images.unsplash.com/photo-1503492362437-648839a90ee4) 50% 50% no-repeat;
        width: 360px;
        height: 320px;
        background-size: cover;
        margin: 20px 20px 70px 0;
        text-align: left;
    }

    .loom>.info>h2 {
        width: 360px;
        padding: 20px;
        background: rgba(255, 255, 255, 1);
        margin-top: 240px;
        font-weight: 400;
    }
    
    .lisatud {
        margin-left: 20px;
    }
    
    @media only screen and (max-width: 1000px) {

        .kuulutused {
            flex-direction: column;
        }
        
        
        .lisatud {
            margin-left: 0;
            order: -1;
        } 
        
    }
    
    @media only screen and (max-width: 830px) {
        .leitud-grid {
            flex-direction: column;
        }
        
    }
    

</style>