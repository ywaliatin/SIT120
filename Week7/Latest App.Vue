<template>
<headertest></headertest>
<router-view></router-view>

<Header/>
<a href="search.html" class="no-underline">
  <img alt="Vue logo" src="./assets/Bublogo.png">
  </a>


<Search/>

<Footer/>
</template>

<script>

import Header from './components/header.vue'
import Search from './components/search.vue'
import Popup from './components/Popup.vue'
import Footer from './components/footer.vue'


export default {
  name:'App',
components: {
    Header,
    Search,
   Popup,
    Footer    
  },
  data() {
    return {
      showPopup: false,
    }
  },
}
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  
}

/* [on big screen] */
/* (A) wrapper */
#hamnav {
    width: 100%;
    background: #8191ad;
}

/* (B) horizontal menu items */
#hamitems { display: flex;}
#hamitems a {
    flex-grow: 1;
    flex-basis: 0;
    padding: 10px;
    color: white;
    text-decoration: none;
    text-align: center;
}

#hamitems a :hover {background: #401408;}

/* (C) hide hamburger */
#hamnav label, #hamburger {display: none;}

/* [on small screen] */
@media screen and (max-width: 769px) {
    /* (A) break into vertical menu */
    #hamitems a {
        box-sizing: border-box;
        display: block;
        width: 100%;
        border-top: 1px solid #333;
    }

    /* (B) show hamburger icon */
    #hamnav label {
        display: inline-block;
        color: white;
        background: #4caf50;
        font-style: normal;
        font-size: 1.2em;
        padding: 10px;
    }

    /* (C) toggle show/hide menu */
    #hamitems {display: none;}
    #hamnav input:checked ~ #hamitems {display: block;}
    
}

.suburb {
  font-family: sans-serif;
  border: 1px solid #eee;
  border-radius: 2px;
  padding: 20px 30px;
  margin-top: 1em;
  margin-bottom: 40px;
  user-select: none;
  overflow-x: auto;
}


</style>
