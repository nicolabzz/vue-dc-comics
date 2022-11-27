<template>
  <header>
    <div class="header-container">
      <div class="img">
        <img src="@/img/dc-logo.png" alt="" srcset="" />
      </div>
      <nav>
        <ul>
          <li
          v-for="eleMenu in arrMenu"
          :key="eleMenu.text"
          >
          <a :href="eleMenu.url">{{ eleMenu.text }}</a>
        </li>
        <!-- old way to list , but wuth v-for is better -->
          <!-- <li><a href="#">Characters</a></li>
          <li><a href="#">comics</a></li>
          <li><a href="#">movies</a></li>
          <li><a href="#">tv</a></li>
          <li><a href="#">games</a></li>
          <li><a href="#">collectibles</a></li>
          <li><a href="#">videos</a></li>
          <li><a href="#">fans</a></li>
          <li><a href="#">news</a></li>
          <li><a href="#">shop</a></li> -->
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderPage',
  data() {
    return {
      arrMenu: [
        {
          url: '#Characters',
          text: 'Characters',
        },
        {
          url: '#comics',
          text: 'comics',
        },
        {
          url: '#movies',
          text: 'movies',
        },
        {
          url: '#tv',
          text: 'tv',
        },
        {
          url: '#games',
          text: 'games',
        },
        {
          url: '#collectibles',
          text: 'collectibles',
        },
        {
          url: '#videos',
          text: 'videos',
        },
        {
          url: '#fans',
          text: 'fans',
        },
        {
          url: '#news',
          text: 'news',
        },
        {
          url: '#shop',
          text: 'shop',
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import '../variables.scss';

header {
  margin: 1rem 0 0 0;
}

.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 1rem auto;
  max-width: $max-width;
  // border: 2px solid black;
}

ul {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100%;
  list-style: none;

  a {
    text-decoration: none;
    margin: 2rem .8rem;
    text-transform: uppercase;
    font-weight: bold;
    color: $text-color;

    &:hover {
      color: $brand-color;
    }
  }
}

// li:nth-child(2) {
//   padding-bottom: 3.3rem;
//   border-bottom: 6px solid $brand-color;
// }

</style>
