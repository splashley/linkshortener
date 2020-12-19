<template>
<div class="Boost">
    <p class="boostText"><strong>Boost your links today</strong></p>
    <button class="getStartedButton">Get Started</button>
    </div>
</template>

<script>
export default {
  name: 'Boost',
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Boost {
    padding: 50px;
    color: white;
    text-align: center;
    background-color: hsl(257, 27%, 26%);
    background-image: url("../assets/bg-boost-mobile.svg");
    background-repeat: no-repeat;
}

.boostText {
    font-size: 20px;
    font-size: 700;
}

.getStartedButton {
    border-radius: 20px;
    background-color: hsl(180, 66%, 49%);
    color: white;
    font-size: 14px;
    font-family: 'Poppins', sans-serif;
    padding: 10px 25px;
    border: none;
}
</style>
