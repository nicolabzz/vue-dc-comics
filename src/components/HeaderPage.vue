<template>
  <header>
    <div class="header-container">
      <div class="img">
        <img src="@/img/dc-logo.png" alt="" srcset="" />
      </div>
      <nav>
        <a href="#">Characters</a>
        <a href="#">comics</a>
        <a href="#">movies</a>
        <a href="#">tv</a>
        <a href="#">games</a>
        <a href="#">collectibles</a>
        <a href="#">videos</a>
        <a href="#">fans</a>
        <a href="#">news</a>
        <a href="#">shop</a>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderPage',
};
</script>

<style lang="scss" scoped>
@import '../variables.scss';

.header-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 1rem auto;
  max-width: $max-width;
  // border: 2px solid black;
}

a {
  text-decoration: none;
  margin: 2rem .8rem;
  border-bottom: 2px solid black;
  text-transform: uppercase;
  font-weight: bold;
}

</style>
