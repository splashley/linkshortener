<template>
  <div id="app">
    <NavBar />
    <TheFooter />
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import TheFooter from './components/TheFooter.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    TheFooter
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@500;700&display=swap');

#app {
margin: 0;
padding: 0;
}

html, body {
  margin: 0;
padding: 0;
font-family: 'Poppins', sans-serif;
font-size: 18px;
}

h1, h2, h3, h4, h5 {
  margin: 0;
  text-align: center;
}
</style>
