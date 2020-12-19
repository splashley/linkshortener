<template>
<div class="Main">
    <div class="AdvancedStats">
<h3>Advanced Statistics</h3>
     <p>Track how your links are performing across the web with our 
  advanced statistics dashboard.</p>
    </div>
<div class="AdvancedDetails">
    <div class="AdvancedDetails-circle">
        <img src="../assets/icon-brand-recognition.svg" class="AdvancedDetails-circle-img">
    </div>
  <h4>Brand Recognition</h4>
  <p>Boost your brand recognition with each click. Generic links don’t 
  mean a thing. Branded links help instil confidence in your content.</p>
  </div>
 <div class="AdvancedDetails-CyanLine"></div>
<div class="AdvancedDetails">
      <div class="AdvancedDetails-circle">
        <img src="../assets/icon-detailed-records.svg" class="AdvancedDetails-circle-img">
    </div>
  <h4>Detailed Records</h4>
  <p>Gain insights into who is clicking your links. Knowing when and where 
  people engage with your content helps inform better decisions.</p>
</div>
 <div class="AdvancedDetails-CyanLine"></div>
<div class="AdvancedDetails">
      <div class="AdvancedDetails-circle">
        <img src="../assets/icon-fully-customizable.svg" class="iconHeight AdvancedDetails-circle-img">
    </div>
  <h4>Fully Customizable</h4>
  <p>Improve brand awareness and content discoverability through customizable 
  links, supercharging audience engagement.</p>
</div>
</div>
</template>

<script>
export default {
  name: 'AdvancedStats',
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.Main {
    display: flex;
    flex-direction: column;
    background-color: rgb(240, 241, 246);
    z-index: -2;
    padding-bottom: 40px;
}

.AdvancedStats {
padding: 20px;
margin-bottom: 40px;
}

.AdvancedStats p {
    font-size: 14px;
    text-align: center;
    color: hsl(257, 7%, 63%);
}

.AdvancedDetails {
    background-color: white;
    border-radius: 7px;
    margin: 0 20px;
    padding: 20px;
    text-align: center;
}
.AdvancedDetails-CyanLine {
    background-color: hsl(180, 66%, 49%);
    width: 7px;
    height: 100px;
    margin: auto;
}

.iconHeight {
    height: 40px;
}

.AdvancedDetails p {
   font-size: 12px;
   line-height: 1.75;
     color: hsl(257, 7%, 63%);
}


.AdvancedDetails-circle {
    display: flex;
    justify-content: center;
    align-items: center;
background-color: hsl(257, 27%, 26%);
border-radius: 50%;
padding: 17px 19px;
margin: -60px auto 20px auto;
max-width: 40px;
text-align: center;
}

.AdvancedDetails-circle-img {

}
</style>
