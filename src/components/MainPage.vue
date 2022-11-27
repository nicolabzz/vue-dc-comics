<template>
  <main>
    <!-- Header top section -->
    <div class="backgroud-dark">

      <!-- Jumbotron full screen section -->
      <div class="jumbotron">
      </div>
      <!-- / Jumbotron full screen section -->

      <!-- Cards Heros Series gri section -->
      <div class="cards-heros-section">
        <span class="badge">CURRENT SERIES</span>
        <CardsHeros
        v-for="objSeries in arrSeries"
        :key="objSeries"
        class="herosCard"
        :imgUrl="objSeries.thumb"
        :title="objSeries.series"

        />
      </div>
      <!-- / Cards Heros Series section -->

    </div>
    <!-- / Header top section -->

    <!-- Blur band with 5 links section  -->
    <div class="blue-band-cardsBg">
      <div class="cards-bar">

        <a href="">
            <div class="card">
              <img src="../img/buy-comics-digital-comics.png" alt="">
            </div>
            <p>DIGITAL COMIX</p>
        </a>
        <a href="">
            <div class="card">
              <img src="../img/buy-comics-merchandise.png" alt="">
            </div>
            <p>DC MERCHANDISE</p>
        </a>
        <a href="">
            <div class="card">
              <img src="../img/buy-comics-subscriptions.png" alt="">
            </div>
            <p>SUBSCRIPTION</p>
        </a>
        <a href="">
            <div class="card">
              <img src="../img/buy-comics-shop-locator.png" alt="">
            </div>
            <p>COMICS SHOP LOCATOR</p>
        </a>
        <a href="">
            <div class="card">
              <img src="../img/buy-dc-power-visa.svg" alt="">
            </div>
            <p>DC POWERED VISA</p>
        </a>

      </div>
    </div>
    <!-- / Blur band with 5 links section  -->
  </main>
</template>
<!-- ======================= -->
<script>
import CardsHeros from '@/components/CardsHeros.vue';

export default {
  name: 'MainPage',
  components: {
    CardsHeros,
  },
  data() {
    return {
      arrSeries: [
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
          price: '$16.99',
          series: 'Aquaman',
          type: 'graphic novel',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$3.99',
          series: 'Batman',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book',
        },
        {
          thumb: 'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel',
        },
      ],
    };
  },
};
</script>
<!-- ======================= -->
<style lang="scss" scoped>
@import '../variables.scss';

.backgroud-dark {
  // border: 2px solid peru;
  background-color: $text-color;
}

.jumbotron {
  background-image: url('../img/jumbotron.jpg');
  height: 550px;
  background-attachment: local;
}

.cards-heros-section {
  // border: 2px solid peru;
  position: relative;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  height: 38rem;
  max-width: $max-width;
  margin: 0 auto;
  padding: 3rem 0;
  // border: 2px solid black

  .badge {
    // border: 2px solid firebrick;
    position: absolute;
    padding: .4rem 2rem;
    background-color: $brand-color;
    color: white;
    top: 0;
    transform: translateY(-50%);
    font-weight: 500;
    font-size: 1.4rem;
  }

  .herosCard {
    flex: 0 0 16.666%;
  }
}

h1 {
  color: white;
}

/*============================
Blur band with 5 links section
==============================*/
.blue-band-cardsBg {
  background-color: $brand-color;

  .cards-bar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 2rem 0;
    max-width: $max-width;
    margin: 0 auto;

    a {
      // border: 2px solid fuchsia;
      display: flex;
      align-items: center;
      text-decoration: none;
      color: white;

      .card {
        // border: 4px solid greenyellow;
        height: 60px;

        img {
          // border: 4px solid goldenrod;
          height: 100%;
        }
      }

      p {
        padding: 0 0 0 1.2rem;
        font-weight: 300;
      }
    }

    a:nth-child(5) {

      .card {
        scale: 0.6;
      }

    };
  }
}

</style>
