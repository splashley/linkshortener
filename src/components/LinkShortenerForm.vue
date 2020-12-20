<template>
<div class="LinkShortenerDiv">
    <form class="LinkShortenerDiv-form">
        <input type="text" placeholder="Shorten a link here..." class="LinkShortenerDiv-form-input">
        <button class="LinkShortenerDiv-form-button">Shorten It!</button>
    </form>
    </div>
</template>

<script>
export default {
  name: 'LinkShortenerForm',
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.LinkShortenerDiv {
    background-color: hsl(257, 27%, 26%);
    background-image: url("../assets/bg-shorten-mobile.svg");
    background-position-x: 100px;
    background-position-y: -20px;
    background-repeat: no-repeat;
    margin: 20px;
    padding: 20px 10px;
    border-radius: 10px;
}

.LinkShortenerDiv-form {
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
    margin: 0 auto;
}

.LinkShortenerDiv-form-input {
    padding: 10px 0 10px 10px;
    font-size: 14px;
    font-family: 'Poppins', sans-serif;
    border-radius: 5px;
    margin-bottom: 17px;
    border: none;
    width: 90%;
        -webkit-box-sizing: border-box; /* Safari/Chrome, other WebKit */
    -moz-box-sizing: border-box;    /* Firefox, other Gecko */
    box-sizing: border-box;         /* Opera/IE 8+ */
}

.LinkShortenerDiv-form-button {
    background-color: hsl(180, 66%, 49%);
    color: white;
    padding: 10px 20px;
    font-size: 16px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    border-radius: 5px;
    border: none;
    width: 90%;
}
</style>
