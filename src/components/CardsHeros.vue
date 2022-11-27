<template>
<div class="card">
  <div class="contents">
    <img
    :src="imgUrl"
    alt="#"
    >
  </div>
  <h3>{{title}}</h3>
</div>
</template>
<!-- ======================= -->
<script>
export default {
  name: 'CardsHeros',
  props: {
    imgUrl: String,
    title: String,
  },
};
</script>
<!-- ======================= -->
<style lang="scss" scoped>
.card {
  padding: .8rem;

  .contents {
    // border: 2px solid fuchsia;
    width: 190px;
    height: 190px;
    overflow: hidden;
  }

  img {
    width:100%;
  }

  h3 {
    color: white;
    font-weight: 300;
    padding: .5rem 0 0 0;
  }
}

</style>
