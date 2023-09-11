<script>
export default {
  props: {
    thumb: String,
    serie: String,
  },
};
</script>

<template>
  <section class="card">
    <a href="">
      <img :src="thumb" alt="" />
      <h6>{{ serie }}</h6>
    </a>
  </section>
</template>

<style lang="scss" scoped>
.card {
  background-color: white;
  width: 150px;
  margin: 20px;

  img {
    width: 100%;
  }
}
</style>
