<template>
<!-- (A) Menu wrapper-->
  <nav id="hamnav">
      <!--(B) the hamburger-->
      <label for="hamburger">&#9776;</label>
          <input type="checkbox" id="hamburger"/>
    
<!-- (C) Menu items-->
   <div id="hamitems">
       
    <router-link to='./components/header.vue'>Search</router-link>
     <a class="active" href="login.vue">Search</a>
    <a class="active" href="login.vue">Login</a>
    <a class="active" href="about.html">About</a>
   </div>    
</nav>

<br>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
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
    #hamitems router-link {
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
</style>
