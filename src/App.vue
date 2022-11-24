<template>
  <div id="app">
    <div id="all-container">
      <HeaderPage />
      <MainPage />
      <FooterPageInfo />
      <FooterPageSocial />
    </div>
  </div>
</template>

<script>
import HeaderPage from '@/components/HeaderPage.vue';
import MainPage from '@/components/MainPage.vue';
import FooterPageInfo from '@/components/Footer/FooterPageInfo.vue';
import FooterPageSocial from '@/components/Footer/FooterPageSocial.vue';

export default {
  components: {
    HeaderPage,
    MainPage,
    FooterPageInfo,
    FooterPageSocial,
  },
};
</script>

<style lang="scss">
@import 'variables.scss';
@import url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');

  * {
    margin:0;
    padding:0;
    box-sizing: border-box;
    font-family: 'Oswald', sans-serif;
  }

  #all-container {
    margin: 0 auto;
  }

  // @font-face {
  //   font-family: Oswald;
  //   src: url('https://fonts.googleapis.com/css2?family=Oswald:wght@200;300;400;500;600;700&display=swap');
  // }
</style>
