<template>
  <main>
    <div class="backgroud-dark">
      <div class="content-goes-here">
        <h1>--&gt;content goese here&lt;--</h1>
      </div>
    </div>
    <div class="cards-bar">
      <div><img src="../img/buy-comics-digital-comics.png" alt=""><p>DIGITAL COMIX</p></div>
      <div><img src="../img/buy-comics-merchandise.png" alt=""><p>DC MERCHANDISE</p></div>
      <div><img src="../img/buy-comics-subscriptions.png" alt=""><p>SUBSCRIPTION</p></div>
      <div><img src="../img/buy-comics-shop-locator.png" alt=""><p>COMICS SHOP LOCATOR</p></div>
      <div><img src="../img/buy-dc-power-visa.svg" alt=""><p>DC POWERED VISA</p></div>
    </div>
  </main>
</template>

<script>
export default {
  name: 'MainPage',
  components: {
  },
  data() {
    return {
      arrHeros: [
        // qui andra' l'array delle cards heros contenenti le informazioni (quwsto l'ho supposto io)
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import '../variables.scss';
.backgroud-dark {
  background-color: $text-color;
}

.content-goes-here {
  display: flex;
  align-items: center;
  height: 8rem;
  max-width: $max-width;
  margin: auto;
  // border: 2px solid black
}

h1 {
  color: white;
}

.cards-bar {
  background-color: $brand-color;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  padding: 2rem 0;
  color: white;

  div:nth-child(4) {
    width: 50px;
    display: flex;

    img {
      width: 100%;
      margin-right: 1rem;
    }
  };

  div:not(:nth-child(4n)) {
    display: flex;
    align-items: center;
    width: 65px;

    img {
      width: 100%;
      margin-right: 1rem;
    }
  };

  div:nth-child(5) {
    width: 85px;
    display: flex;

    img {
      width: 100%;
      margin-right: 1rem;
    }
  };
}

</style>
