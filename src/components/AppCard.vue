<script>
export default {
  props: {
    thumb: String,
    serie: String,
  },
};
</script>

<template>
  <!-- card -->
  <section>
    <a href="">
      <div class="card">
        <img class="card-img" :src="thumb" alt="" />
      </div>
      <h6>{{ serie }}</h6>
    </a>
  </section>
</template>

<style lang="scss" scoped>
section {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 25%;
  color: white;

  a {
    text-align: center;
    text-decoration: none;
    color: currentColor;
  }
  h6 {
    margin: 10px 0;
    max-width: 150px;
  }
}
.card {
  max-width: 150px;
  aspect-ratio: 1;
  overflow: hidden;
}

img {
  background-color: white;
  width: 100%;
}
</style>
