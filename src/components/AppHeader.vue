<script>
export default {
  data() {
    return {
      links: [
        {
          text: "character",
          url: "#",
          current: false,
        },
        {
          text: "comics",
          url: "#",
          current: false,
        },
        {
          text: "movies",
          url: "#",
          current: false,
        },
        {
          text: "tv",
          url: "#",
          current: false,
        },
        {
          text: "games",
          url: "#",
          current: false,
        },
        {
          text: "collectables",
          url: "#",
          current: false,
        },
        {
          text: "videos",
          url: "#",
          current: false,
        },
        {
          text: "fan",
          url: "#",
          current: false,
        },
        {
          text: "news",
          url: "#",
          current: false,
        },
        {
          text: "shop",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <header>
    <ul>
      <li v-for="link in links">
        <a :href="link.url">
          {{ link.text }}
        </a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped></style>
