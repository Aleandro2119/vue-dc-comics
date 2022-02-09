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

        <div class="bg-dc">
          <img class="logo-dc" src="../assets/dc-logo-bg.png" alt="Logo Dc" />
        </div>
      </div>
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

  .bg-dc {
    position: relative;
    left: 250px;
  }

  a {
    color: #797979;
    text-decoration: none;
  }
  .position {
    display: flex;

    h4 {
      padding: 40px 0;
      font-size: 18px;
      color: white;
    }

    ul {
      padding-right: 15px;

      li {
        list-style-type: none;
        padding: 5px 0;
        font-size: 12px;
      }
    }
  }
}
</style>