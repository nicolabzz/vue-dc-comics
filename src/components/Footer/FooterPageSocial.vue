<template>
<footer>
<div class="footerSocial-container">
  <div class="singUp-social">
    <div class="sing-up-section">
      <h3>SING-UP NOW!</h3>
    </div>
    <div class="social-section">
      <h3>FOLLOW US</h3>
      <img src="../../img/footer-facebook.png" alt="">
      <img src="../../img/footer-twitter.png" alt="">
      <img src="../../img/footer-youtube.png" alt="">
      <img src="../../img/footer-pinterest.png" alt="">
      <img src="../../img/footer-periscope.png" alt="">
    </div>
  </div>
</div>
</footer>
</template>

<script>
export default {
  name: 'FooterPageSocial',
};
</script>

<style lang="scss" scoped>
@import '../../variables.scss';

.footerSocial-container{
  // border: 2px solid greenyellow;
  background-color: $footer-color;
  height: 10rem;
  display: flex;
  justify-content: center;
  align-items: center;

  .singUp-social {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 100%;
    max-width: $max-width;
  };

  .sing-up-section {
    border: 2px solid $brand-color;
    padding: 1rem;
    color: white;
  }

  .social-section {
   color: $brand-color;
    display:flex;
    flex-direction: columns;
    gap: 1rem;
  };
}
  </style>
