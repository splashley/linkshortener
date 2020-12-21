<template>
<div class="GetStarted-Div">
        <div class="GetStarted-Div-Text-Desktop">
        <h2>More than just shorter links</h2>

  <p>Build your brand’s recognition and get detailed insights 
  on how your links are performing.</p>
<button class="GetStarted-Div-Text-Button">Get Started</button>
    </div>
    <div class="GetStarted-Div-Image">
        <img src="../assets/illustration-working.svg" class="GetStarted-Div-Image-Svg">
    </div>
    <div class="GetStarted-Div-Text">
        <h2>More than just shorter links</h2>

  <p>Build your brand’s recognition and get detailed insights 
  on how your links are performing.</p>
<button class="GetStarted-Div-Text-Button">Get Started</button>
    </div>
    </div>
</template>

<script>
export default {
  name: 'GetStarted',
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.GetStarted-Div {
    display: flex;
    flex-direction: column;
}

.GetStarted-Div-Text-Desktop {
    display: none;
}

.GetStarted-Div-Image {
text-align: right;
}

.GetStarted-Div-Image-Svg {
 width: 100vw;
 height: auto;
 /* margin-right: -70px; */
}
.GetStarted-Div-Text {
    padding: 20px;
    text-align: center;
}

.GetStarted-Div-Text h2 {
    color: hsl(255, 11%, 22%);
    font-size: 34px;
    font-family: 'Poppins', sans-serif;
    letter-spacing: -0.10rem;
    font-weight: 700;
    line-height: 1.2;
}
.GetStarted-Div-Text p {
    color: hsl(257, 7%, 63%);
    font-size: 14px;
}
.GetStarted-Div-Text-Button {
        background-color: hsl(180, 66%, 49%);
    color: white;
    padding: 10px 35px;
    font-size: 16px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    border-radius: 25px;
    border: none;
    margin-top: 10px;
    margin-bottom: 30px;
}

@media only screen and (min-width: 375px) {

    .GetStarted-Div {
    display: flex;
    flex-direction: row;
    padding: 50px;
    overflow: hidden;
}

.GetStarted-Div-Text-Desktop {
    display: flex;
    flex-direction: column;
    padding-right: 80px;
}

.GetStarted-Div-Text {
    display: none;
}

.GetStarted-Div-Image-Svg {
 width: 60vw;
 height: auto;
 margin-right: -110px;
 padding-left: 20px;
}

.GetStarted-Div-Text-Desktop h2 {
    text-align: left;
    color: hsl(255, 11%, 22%);
    font-size: 40px;
    font-family: 'Poppins', sans-serif;
    letter-spacing: -0.10rem;
    font-weight: 700;
    line-height: 1.1;
}

.GetStarted-Div-Text-Desktop p {
    text-align: left;
    color: hsl(257, 7%, 63%);
    font-size: 14px;
    font-family: 'Poppins', sans-serif;
    font-weight: 300;
    line-height: 1.4;
}

.GetStarted-Div-Text-Button {
        background-color: hsl(180, 66%, 49%);
    color: white;
    padding: 10px 20px;
    font-size: 16px;
    font-family: 'Poppins', sans-serif;
    font-weight: 700;
    border-radius: 25px;
    border: none;
    width: 200px;
    margin: 0;
}
}
</style>
