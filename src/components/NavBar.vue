<template>
 <header>
   <div class="Logo">
     <img src="../assets/logo.svg">
   </div>
   <div class="NavBar-Desktop">
     <div class="NavBar-Desktop-Left">
     <a href="">Features</a>
     <a href="">Pricing</a>
     <a href="">Resources</a>
     </div>
     <div class="NavBar-Desktop-Right">
     <a href="">Login</a>
     <button class="HamburgerMenu-Links-SignupButton">Sign Up</button>
     </div>
     </div>
  <div class="HamburgerMenu" @click="showMenu = !showMenu">
     <div class="HamburgerIcon"></div>
     <div class="HamburgerIcon"></div>
     <div class="HamburgerIcon"></div>
     </div>
   <div class="HamburgerMenu-OutsideLayer">
     <div v-if="showMenu" id="HamburgerMenu-Links">
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
  data() {
    return {
      showMenu: false
    }
  },
  methods: {}
}
  
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

/* 
 I can't explain exactly why the position: absolute affects this, but when you use it, the width doesn't "squish" with padding/margin. If you used position: relative (which you can't here because it's a menu overlaying stuff), then the width: 100% would auto-calculate to be the width of the screen - padding - margin. */


@media only screen and (min-width: 500px) {


  .HamburgerMenu {
    display: none;
  }

  #HamburgerMenu-Links {
  display: none;
}


  .NavBar-Desktop {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
  }

  .NavBar-Desktop-Right  {
    display: flex;
    flex-direction: row;
    align-items: center;
  }

  .NavBar-Desktop-Left {
    float: left;
  }

  .NavBar-Desktop-Left a {
    text-decoration: none;
    font-size: 16px;
    color: hsl(257, 7%, 63%);
    padding: 0 10px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
  }

    .NavBar-Desktop-Right a {
    text-decoration: none;
    color: hsl(257, 7%, 63%);
    padding: 0 10px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    font-size: 16px;
  }

  .HamburgerMenu-Links-SignupButton {
   background-color: hsl(180, 66%, 49%);
    color: white;
    padding: 5px 10px;
    font-size: 16px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    border-radius: 15px;
    border: none;
    width: 90%;
    margin: 0 auto;
}
}

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
    width: calc(100vw - 35px);
}

#HamburgerMenu-Links {
  display: flex;
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

</style>
