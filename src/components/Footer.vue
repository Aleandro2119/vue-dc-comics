<template>
  <footer>
    <div class="container">
      <div class="position">
        <nav>
          <h4>DC COMICS</h4>
          <ul>
            <li v-for="(comic, index) in comics" :key="index">
              <a :href="comic.url">{{ comic.text }}</a>
            </li>
          </ul>
        </nav>

        <nav>
          <h4>SHOP</h4>
          <ul>
            <li v-for="(shop, index) in shop" :key="index">
              <a :href="shop.url">{{ shop.text }}</a>
            </li>
          </ul>
        </nav>

        <nav>
          <h4>DC</h4>
          <ul>
            <li v-for="(dc, index) in dc" :key="index">
              <a :href="dc.url">{{ dc.text }}</a>
            </li>
          </ul>
        </nav>

        <nav>
          <h4>SITES</h4>
          <ul>
            <li v-for="(site, index) in sites" :key="index">
              <a :href="site.url">{{ site.text }}</a>
            </li>
          </ul>
        </nav>
      </div>
      <div class="bg-dc"></div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      comics: [
        { text: "Characters", url: "#" },
        { text: "Comics", url: "#" },
        { text: "Movies", url: "#" },
        { text: "TV", url: "#" },
        { text: "Games", url: "#" },
        { text: "Videos", url: "#" },
        { text: "News", url: "#" },
      ],

      shop: [
        { text: "Shop DC", url: "#" },
        { text: "Shop DC Collectibles", url: "#" },
      ],

      dc: [
        { text: "Terms Of Use", url: "#" },
        { text: "Privacy policy (New)", url: "#" },
        { text: "Ad Choices", url: "#" },
        { text: "Advertising", url: "#" },
        { text: "Jobs", url: "#" },
        { text: "Subscriptions", url: "#" },
        { text: "Talent Workshops", url: "#" },
        { text: "CPSC Certificates", url: "#" },
        { text: "Ratings", url: "#" },
        { text: "Shop Help", url: "#" },
        { text: "Contact Us", url: "#" },
      ],

      sites: [
        { text: "DC", url: "#" },
        { text: "MAD Magazine", url: "#" },
        { text: "DC Kids", url: "#" },
        { text: "DC Universe", url: "#" },
        { text: "DC Power Visa", url: "#" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
footer {
  background-image: url("../assets/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;

  .position {
    display: flex;
    flex-wrap: wrap;

    h4 {
      color: white;

      li {
        list-style-type: none;

        a {
          color: lightslategray;
          font-size: 12px;
          text-decoration: none;
        }
      }
    }
  }
}

.bg-dc {
  background-image: url("../assets/dc-logo-bg.png");
}
</style>