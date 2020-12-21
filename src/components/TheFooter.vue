<template>
 <div class="Footer">
<h2 class="h2-logo">Shortly</h2>
   <ul class="footer-links">
 <li class="footer-links-titles">Features</li>
  <li class="footer-links-a">Link Shortening</li>
 <li class="footer-links-a"> Branded Links</li>
  <li class="footer-links-a">Analytics</li>
    </ul>
       <ul class="footer-links">
  <li class="footer-links-titles">Resources</li>
  <li class="footer-links-a">Blog</li>
  <li class="footer-links-a">Developers</li>
  <li class="footer-links-a">Support</li>
    </ul>
     <ul class="footer-links">
 <li class="footer-links-titles">Company</li>
  <li class="footer-links-a">About</li>
 <li class="footer-links-a"> Our Team</li>
  <li class="footer-links-a">Careers</li>
  <li class="footer-links-a">Contact</li>
  </ul>
  <ul class="social-media">
    <li><img src="../assets/icon-facebook.svg"></li>
    <li><img src="../assets/icon-twitter.svg"></li>
    <li><img src="../assets/icon-pinterest.svg"></li>
    <li><img src="../assets/icon-instagram.svg"></li>
    </ul>
   </div>
</template>

<script>
export default {
  name: 'TheFooter',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.Footer {
  color: white;
  text-align: center;
  background-color: hsl(260, 8%, 14%);
  margin: 0;
  width: 100%;
  padding: 30px 0;
}

ul {
  list-style: none;
  padding: 0;
  }

.footer-links li {
  line-height: 1.5;
  padding-bottom: 10px;
}

.footer-links-titles {
  font-size: 14px;
}

.footer-links-a {
  font-size: 12px;
}

.social-media li {
  display: inline;
  padding: 0 10px;
}

@media only screen and (min-width: 375px) {
 .Footer {
display: flex;
margin: 0 auto;
padding: 50px 0;
justify-content: center;
}

.h2-logo {
  padding-right: 150px;
}

.footer-links {
  margin: 0 50px;
  text-align: left;
}

}
</style>
