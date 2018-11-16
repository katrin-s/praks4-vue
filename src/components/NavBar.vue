<template>
  <div class="hello">
   <header>
       <nav>
         <img style="cursor: pointer;" onclick="window.location='/';" src="https://images.vexels.com/media/users/3/139889/isolated/preview/da50fec14dc402a17863b78227684335-cat-silhouette-2-by-vexels.png" alt="Varjupaiga logo">
         <ul>
           <li><router-link to="/">avaleht</router-link></li><li><router-link to= "/loomad">loomad varjupaigas</router-link></li><li>
            <router-link to="/leitud">kadunud/leitud</router-link>
            </li><li><router-link to="/toetamine">kuidas toetada?</router-link>
            </li><li><router-link to="/meist">meist</router-link>
            </li><li><router-link to="/kontakt">kontakt</router-link></li>
         </ul>
      </nav>
      <section class="mobile" v-if="showNav">
         <ul>
           <li style="cursor: pointer;" onclick="window.location='/';"><h2>avaleht</h2></li><li><router-link to= "/loomad"><h2>loomad varjupaigas</h2></router-link></li><li>
            <router-link to="/leitud"><h2>kadunud/leitud</h2></router-link>
            </li><li><router-link to="/toetamine"><h2>kuidas toetada?</h2></router-link>
            </li><li><router-link to="/meist"><h2>meist</h2></router-link>
            </li><li><router-link to="/kontakt"><h2>kontakt</h2></router-link></li>
            <a class="closing" href="#" @click="closeNav()"><h2>&#215;</h2></a>
         </ul>
      </section>
      <div class="clearfix"></div>
      <div class="hamburger" @click="openNav()">
     <a href="#"><span></span>
      <span></span>
       <span></span></a>
        </div><div class="clearfix"></div>
   </header>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
  data() {
    return {
      showNav: false,
    };
  },
  methods: {
    openNav() {
      this.showNav = true;
    },
    closeNav() {
      this.showNav = false;
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hamburger {
    display: none;
}
    .mobile {
        display: none;
    }

header {
    text-align: center;
    width: 100%;
    height: 100px;
    position: fixed;
    top: 0;
    z-index: 3;
    color: white;
    background-color: #1CAAAA;
}

nav {
    display: block;
    width: 89%;
    overflow: hidden;
    margin-left: auto;
    margin-right: auto;
    font-weight: 700;
}

nav img {
    height: 60px;
    width: 60px;
    border-radius: 50%;
    margin-top: 20px;
    object-fit: cover;
    float: left;
    background-color: white;
}

nav ul {
    float: right;
    display: flex;
}

nav ul li {
    text-decoration: none;
    text-transform: uppercase;
    padding: 40px 10px;
}

nav a {
    text-decoration: none;
    color: white;
    background-color: transparent;
}

nav a:hover {
    border-bottom: 2px solid white;
}

.router-link-exact-active {
    background-color: rgba(255, 255, 255, 0.7);
    color: black;
    padding: 10px 20px;
    border: none;
    border-radius: 30px;
}

@media only screen and (max-width: 1240px) {
    nav a {
    display: none;
    }
    .hamburger {
        display: block;
        float: right;
        margin-top: -40px;
        margin-right: 6%;
        position: relative;
}
    .mobile {
        display: block;
        width: 100vw;
        height: 100vh;
        background-color: #1CAAAA;
    }
    .mobile ul {
        display: flex;
        flex-direction: column;
        padding-top: 40px;
    }
    .mobile h2 {
        margin-bottom: 30px;
    }
    .mobile a {
        text-decoration: none;
        color: white;
    }

    .hamburger span {
        background: white;
        width: 30px;
        height: 5px;
        display: block;
        margin-bottom: 4px;
}
    .closing h2 {
        font-size: 50px;
    }
    .router-link-exact-active {
    background-color: rgba(255, 255, 255, 0);
    padding: 0;
}
    }

</style>
