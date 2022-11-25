<template>
  <footer>
    <div class="background-conainer">
      <div class="container-info-bigLogo">
          <div class="box-info">
            <h3>DC COMICS</h3>
            <ul>
              <li>Characters</li>
              <li>Comix</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
          </div>
          <div class="box-info">
            <h3>SHOP</h3>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
          <div class="box-info">
            <h3>DC</h3>
            <ul>
              <li>Terms Of Use</li>
              <li>Pryvacy policy (New)</li>
              <li>Ad Chioices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscription</li>
              <li>Talent Workshop</li>
              <li>CPSC Certificate</li>
              <li>Ratings</li>
              <li>Shop help</li>
              <li>Contact Us</li>
            </ul>
          </div>
          <div class="box-info">
            <h3>SITES</h3>
            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        <div class="bigLogo">
          <img src="../../img/dc-logo-bg.png" alt="">
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'footerPsgeInfo',
};
</script>

<style lang="scss" scoped>
@import '../../variables.scss';

footer {
  background-image: url('../../img/footer-bg.jpg');
  height: 482px;
  max-width: 1900px;
  margin: auto;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

.background-conainer {
  // border: 2px solid green;
  width: 100%;
  height: 482px;
  max-width: $max-width;
  flex-flow: column wrap;
  display: flex;
  margin: auto;
}

.container-info-bigLogo {
  // border: 2px solid royalblue;
  max-width: 1900px;
  height: 482px;
  display: flex;
  flex-direction: column;
  flex-wrap: wrap;
  color: white;
}

.box-info {
  // border: 2px solid crimson;
  padding: 2rem 0;
  flex: 1 1 80px;

  h3 {
    margin-bottom: 1rem;
  }

  ul {
    list-style-type: none;
  }
}

.bigLogo {
  // border: 2px solid fuchsia;
  flex: 1 1 80px;
  height: 300px;

  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  };
}

</style>
