<script>
import AppHeader from "./components/AppHeader.vue";
import AppMainContent from "./components/AppMainContent.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: { AppHeader, AppMainContent, AppFooter },
};
</script>

<template>
  <!-- <div class="container"> -->
  <div class="">
    <AppHeader />
    <AppMainContent />
    <AppFooter />
  </div>
</template>

<style lang="scss">
@use "./assets/styles/general.scss";
</style>
