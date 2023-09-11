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
      <li>
        <img src="../assets/dc-logo.png" alt="" />
      </li>
      <li v-for="link in links">
        <a :href="link.url">
          {{ link.text }}
        </a>
      </li>
    </ul>
  </header>
</template>

<style lang="scss" scoped>
header {
  background-color: white;
  height: 100px;
  line-height: 100px;
}

ul {
  display: flex;
  justify-content: end;
  align-items: center;
  gap: 10px;
  li {
    display: inline-block;
    text-decoration: none;
    list-style: none;

    &:first-child {
      flex-grow: 1;
      margin: 0 30px;
    }
    &:hover {
      color: blue;
      border-bottom: 1px solid blue;
      padding-bottom: 10px;
    }
  }

  a {
    text-decoration: none;
    color: currentColor;
  }

  img {
    width: 50px;
    display: block;
  }
}
</style>
