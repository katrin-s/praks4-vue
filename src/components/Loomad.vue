<template>
  <div class="hello">
     <section class="loomad">
            <h2>LOOMAD VARJUPAIGAS</h2>
            <div class="filter">
                <div class="liik">
                <button type="button">KASSID</button>
                <button type="button">KOERAD</button>
                <button type="button">K&Otilde;IK</button>
                </div>
                <div class="otsing">
                <form action="">
                    <input type="text" placeholder=" Otsi nime või ID järgi...">
                </form>
                <button type="button">OTSI</button>
                </div>
            </div>
            <div class="loomad-grid">
                <a href="#" @click="openModal()"><div class="loom-1"><h2>MURI</h2></div></a>
                <a href="#"><div class="loom-2"><h2>joosep</h2></div></a>
                <a href="#"><div class="loom"><h2>KASS</h2></div></a>
                <a href="#"><div class="loom"><h2>KASS</h2></div></a>
            </div>
             <div>
           <button id="go-up">&#94; &Uuml;LES</button>
       </div>
   </section>
  <div class="modal-backdrop" v-if="showModal">
        <!--
on mobile change image and info order, text first
drop shadow for box, darker background
-->
        <div class="profiilipopup">
            <a class="closing" href="#" @click="closeModal()"><h2>&#215;</h2></a>
            <div class="nupud">
                <a class="previous" href="#"><h2>&#60; eelmine</h2></a>
                <a class="next" href="#"><h2>j&Auml;rgmine &#62;</h2></a>
            </div>
            <div class="profiil">
                <div class="profiilipilt">
                    <img src="https://images.unsplash.com/photo-1533981254884-914bdb5000fa?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=c66c07ab743280f06cfa7e4ad7c3890f&auto=format&fit=crop&w=1950&q=80" alt="puppy in snow">
                </div>
                <div class="andmed">
                    <h3>muri</h3>
                    <h2>id: 123456</h2>
                    <table>
                        <tr>
                            <td>Liik:</td>
                            <td>Koer</td>
                        </tr>
                        <tr>
                            <td>Vanus:</td>
                            <td>6 kuud</td>
                        </tr>
                        <tr>
                            <td>Sugu:</td>
                            <td>Isane</td>
                        </tr>
                        <tr>
                            <td>Ster./kast.:</td>
                            <td>Ei</td>
                        </tr>
                        <tr>
                            <td>Varjupaigas alates:</td>
                            <td>12.12.2018</td>
                        </tr>
                    </table>
                    <p class="kirjeldus">
                        Rämsi külast võõra talu õuelt leitud
                        kutsikas, isegi kaelarihm oli kaelas. Kahtlus on, et keegi ta sinna poetas.
                        <br>
                        Tundub terve ja tragi, väga sotsiaalne ning kindlasti kasvab temast suur koer.
                        <br>
                        <br>
                        Huvi korral võta ühendust:
                        <br>
                        <br>
                        +372 7 361 866
                        <br>
                        info@khk.ee
                    </p>
                </div>
            </div>
        </div>
    </div>
    </div>
</template>

<script>
export default {
  name: 'Loomad',
   data() { 
    return { 
      showModal: false 
    } 
  },
    methods: { 
   openModal() { 
     this.showModal = true; 
   },
    closeModal() {
     this.showModal = false;
  },
 } 
};
    
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .loomad {
    margin: 120px auto 0 auto;
    width: 89%;
    display: flex;
    flex-direction: column;
    text-align: center;
}

.loomad>h2 {
    padding-bottom: 20px;
}

.filter {
    display: flex;
    justify-content: flex-start;
}

.liik {
    display: flex;
}

.otsing {
    display: flex;
}

.otsing>form {
    margin-right: 10px;
    margin-left: 30px;
    display: inline;
    padding-top: 4px;
}

.otsing>form>input {
    width: 240px;
    height: 34px;
    border: none;
    font-size: 14px;
}

.loomad-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: flex-start;
    align-content: center;
}
.loomad-grid a {
    text-decoration: none;
    color: black;
}
.loom {
    background: url(https://images.unsplash.com/photo-1533738699159-d0c68059bb61?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=0bb9888db1d270eab08c77f41120dfca&auto=format&fit=crop&w=634&q=80) 50% 50% no-repeat;
    width: 250px;
    height: 250px;
    margin: 20px;
    text-align: center;
}
.loom-1 {
    background: url(https://images.unsplash.com/photo-1533981254884-914bdb5000fa?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=c66c07ab743280f06cfa7e4ad7c3890f&auto=format&fit=crop&w=1950&q=80) 50% 50% no-repeat;
    width: 250px;
    height: 250px;
    margin: 20px;
    text-align: center;
    }
.loom>h2 {
    width: 250px;
    padding-top: 20px;
    padding-bottom: 20px;
    background: rgba(255, 255, 255, 0.6);
    margin-top: 10px;
}
.loom-1>h2 {
     width: 250px;
     padding-top: 20px;
     padding-bottom: 20px;
     background: rgba(255, 255, 255, 0.6);
     margin-top: 10px;
}
.loom-2 {
    background: url(https://images.unsplash.com/photo-1506160484494-d2b1d999debd?ixlib=rb-0.3.5&ixid=eyJhcHBfaWQiOjEyMDd9&s=758725217d05454551484dc0c92d3a03&auto=format&fit=crop&w=500&q=60) 50% 50% no-repeat;
    width: 250px;
    height: 250px;
    margin: 20px;
    text-align: center;
    }
.loom-2>h2 {
    width: 250px;
    padding-top: 20px;
    padding-bottom: 20px;
    background: rgba(255, 255, 255, 0.6);
    margin-top: 10px;
}
      @media only screen and (max-width: 700px) {
    .filter {
        flex-direction: column;
    }
    .otsing {
        margin-top: 20px;
    }
    .otsing>form {
    margin-left: 0;
}
}
 .modal-backdrop {
        position: fixed;
        top: 0;
        bottom: 0;
        left: 0;
        right: 0;
        background-color: rgba(0, 0, 0, 0.3);
        display: flex;
        justify-content: center;
        align-items: center;
     z-index: 3;}
    .profiilipopup {
        width: 1000px;
        height: 100vh;
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: auto;
        background-color: white;
        overflow-y: auto;
        line-height: 150%;
    }
    .profiilipilt img {
        width: 600px;
        height: auto;
        margin-bottom: 10px;
    }
    .nupud {
        display: flex;
        align-self: center;
        margin-bottom: 20px;
    }
    .closing {
        text-decoration: none;
        align-self: flex-end;
    }
    .next {
        margin-left: 40px;
    }
    .closing h2 {
        color: black;
        font-size: 70px;
        margin-right: 20px;
        margin-top: 20px;
    }
    h3 {
        text-transform: uppercase;
    }
    .profiil {
        display: flex;
        margin-bottom: 20px;
    }
    .andmed {
        margin-left: 20px;
        width: 360px;}
    @media only screen and (max-width: 1060px) {
        .profiilipopup {
            width: 700px;
    }
        .profiil {
            flex-direction: column;
    }
        .andmed {
            order: -1;
            margin-left: 0;
            width: 600px;
        }
    }
    @media only screen and (max-width: 730px) {
        .profiilipopup {
            width: 90vw;
        }

        .profiil {
            flex-direction: column;
        }

        .andmed {
            order: -1;
            margin-left: 0;
            width: 80vw;
        }
        .profiilipilt img {
            width: 80vw;
        }
        .next {
            margin-left: 20px;
        }
    }
</style>
