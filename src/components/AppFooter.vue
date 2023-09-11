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
      shops: [
        {
          text: "Shop DC",
          url: "#",
          current: false,
        },
        {
          text: "Shop DC Collectables",
          url: "#",
          current: false,
        },
      ],
      dcTerms: [
        {
          text: "Terms of use",
          url: "#",
          current: false,
        },
        {
          text: "Privacy policy (new)",
          url: "#",
          current: false,
        },
        {
          text: "Add choices",
          url: "#",
          current: false,
        },
        {
          text: "Advertising",
          url: "#",
          current: false,
        },
        {
          text: "Jobs",
          url: "#",
          current: false,
        },
        {
          text: "Subscriptions",
          url: "#",
          current: false,
        },
        {
          text: "Talent Workshop",
          url: "#",
          current: false,
        },
        {
          text: "CPSC certificates",
          url: "#",
          current: false,
        },
        {
          text: "Rating",
          url: "#",
          current: false,
        },
        {
          text: "Shop help",
          url: "#",
          current: false,
        },
        {
          text: "Contact us",
          url: "#",
          current: false,
        },
      ],
      sites: [
        {
          text: "DC",
          url: "#",
          current: false,
        },
        {
          text: "Mad Magazine",
          url: "#",
          current: false,
        },
        {
          text: "Dc Kids",
          url: "#",
          current: false,
        },
        {
          text: "DC universe",
          url: "#",
          current: false,
        },
        {
          text: "DC power Visa",
          url: "#",
          current: false,
        },
      ],
    };
  },
};
</script>

<template>
  <footer>
    <!-- sezione dei links -->
    <section id="footer-links">
      <div class="list-Container">
        <ul>
          <h5>DC COMICS</h5>
          <li v-for="link in links">
            <a :href="link.url">
              {{ link.text }}
            </a>
          </li>
          <h5>SHOP</h5>
          <li v-for="shop in shops">
            <a :href="shop.url">
              {{ shop.text }}
            </a>
          </li>
        </ul>
        <ul>
          <h5>DC</h5>
          <li v-for="dcTerm in dcTerms">
            <a :href="dcTerm.url">
              {{ dcTerm.text }}
            </a>
          </li>
        </ul>
        <ul>
          <h5>SITES</h5>
          <li v-for="site in sites">
            <a :href="site.url">
              {{ site.text }}
            </a>
          </li>
        </ul>
      </div>
    </section>
    <!-- sezione sign up now -->
    <section id="footer-social">
      <h5>ALTRO</h5>
      <!--  -->
    </section>
  </footer>
</template>

<style lang="scss" scoped>
h5 {
  padding: 10px 0;
}

#footer-links {
  padding: 30px;
  color: white;
  background-image: url(../assets/footer-bg.jpg);

  .list-Container {
    display: flex;
    justify-content: start;

    ul {
      margin: 0 20px;
      text-decoration: none;
      list-style: none;
      li {
        font-size: smaller;
        color: grey;
      }
    }
    a {
      text-decoration: none;
      color: currentColor;
    }
  }
}

#footer-social {
  color: white;
  background-color: gray;
}
</style>
