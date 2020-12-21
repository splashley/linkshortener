<template>
 <header>
   <div class="Logo">
     <img src="../assets/logo.svg">
   </div>
   <div class="NavBar-Desktop">
     <div class=""></div>
     <div class=""></div>
     </div>
   <div class="HamburgerMenu">
     <a href="javascript:void(0);" v-on:click="myFunction()">
     <div class="HamburgerIcon"></div>
     <div class="HamburgerIcon"></div>
     <div class="HamburgerIcon"></div>
     </a>
   </div>
   <div class="HamburgerMenu-OutsideLayer">
   <div id="HamburgerMenu-Links">
     <a href="">Features</a>
     <a href="">Pricing</a>
     <a href="">Resources</a>
     <div class="HamburgerMenu-Links-Line"></div>
     <a href="">Login</a>
     <button class="HamburgerMenu-Links-SignupButton">Sign Up</button>
   </div>
   </div>
   </header>
</template>

<script>
export default {
  name: 'NavBar',
  methods: {
  myFunction() {
  const x = document.getElementById("HamburgerMenu-Links");
  if (x.style.display === "flex") {
    x.style.display = "none";
  } else {
    x.style.display = "flex";
  }
    }
  }
}
  
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/* 
 I can't explain exactly why the position: absolute affects this, but when you use it, the width doesn't "squish" with padding/margin. If you used position: relative (which you can't here because it's a menu overlaying stuff), then the width: 100% would auto-calculate to be the width of the screen - padding - margin. */

header {
  padding: 30px 20px 30px 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.Logo {
  padding-left: 30px;
}

.NavBar-Desktop {
  display: none;
}
.HamburgerIcon {
    width: 30px;
  height: 3px;
  background-color: hsl(257, 7%, 63%);
  margin: 6px 0;
}

.HamburgerMenu-OutsideLayer {
  position: absolute;
    top: 90px;
    padding: 10px;
    width: calc(100vw - 20px);
}

#HamburgerMenu-Links {
  display: none;
  flex-direction: column;
  justify-content: center;
  align-content: center;
  background-color: hsl(257, 27%, 26%);
  border-radius: 15px;
  color: white;
  font-family: 'Poppins', sans-serif;
  font-weight: 700;
  text-align: center;
  line-height: 2;
  padding: 30px 0;
}


#HamburgerMenu-Links a {
  color: white;
  text-decoration: none;
  font-size: 18px;
  padding: 15px 0;
}

.HamburgerMenu-Links-Line {
  height: 1px;
  background-color: hsl(0, 0%, 75%);
  width: 90%;
  margin: 0 auto;
}
.HamburgerMenu-Links-SignupButton {
   background-color: hsl(180, 66%, 49%);
    color: white;
    padding: 10px 20px;
    font-size: 18px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    border-radius: 20px;
    border: none;
    width: 90%;
    margin: 0 auto;
}

@media only screen and (min-width: 375px) {
  .HamburgerMenu {
    display: none;
  }
}
</style>
