<template>
  <div class="hello">
    <header>
      <nav>
         <img src="https://images.vexels.com/media/users/3/139889/isolated/preview/da50fec14dc402a17863b78227684335-cat-silhouette-2-by-vexels.png" alt="Varjupaiga logo">
         <ul>
            <li><router-link to="/">avaleht</router-link></li><li><router-link to= "/loomad">loomad varjupaigas</router-link></li><li>
            <router-link to="/leitud">kadunud/leitud</router-link>
            </li><li><router-link to="/toetamine">kuidas toetada?</router-link>
            </li><li><router-link to="/meist">meist</router-link>
            </li><li><router-link to="/kontakt">kontakt</router-link></li>
         </ul> 
      </nav>
      <div class="clearfix"></div>
		<div class="hamburger">
			<span></span>
			<span></span>
			<span></span>
		</div>
		<div class="clearfix"></div>  
   </header>
  </div>
</template>

<script>
export default {
  name: 'NavBar',
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    
.hamburger {
    display: none;
}

header {
    text-align: center;
    width: 100%;
    background-color: white;
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
    background-color: rgba(255, 255, 255, 0.9);
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

    .hamburger span {
	background: white;
	width: 30px;
	height: 5px;
	display: block;
	margin-bottom: 4px;
}
    }

</style>