<template>
  <main>
    <div class="container">
      <nav>
        <ul>
          <li v-for="shop in shops" :key="shop.text">
            <a href="#"
              ><img :src="require(`../assets/${shop.image}`)" alt="Shop" />
              <span>{{ shop.text }}</span>
            </a>
          </li>
        </ul>
      </nav>
    </div>
  </main>
</template>

<script>
export default {
  name: "MainTop",

  data() {
    return {
      shops: [
        {
          text: "DIGITAL COMICS",
          image: "buy-comics-digital-comics.png",
          url: "#",
        },
        {
          text: "DC MERCHANDISE",
          image: "buy-comics-merchandise.png",
          url: "#",
        },
        {
          text: "SUBSCRIPTION",
          image: "buy-comics-subscriptions.png",
          url: "#",
        },
        {
          text: "COMIC SHOP LOCATOR",
          image: "buy-comics-shop-locator.png",
          url: "#",
        },
        {
          text: "DC POWER VISA",
          image: "buy-dc-power-visa.svg",
          url: "#",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  max-width: 1100px;
  margin: 0 auto;
}

main {
  background-color: #0282f9;
  padding: 10px;

  ul {
    display: flex;
    align-items: center;

    li {
      list-style-type: none;
      padding: 40px;
    }

    a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: white;
      font-size: 12px;

      span {
        padding-left: 5px;
        font-size: 12px;
      }

      img {
        width: 25%;
      }
    }
  }
}
</style>