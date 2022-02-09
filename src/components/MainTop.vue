<template>
  <header>
    <div class="container">
      <nav>
        <ul>
          <li>
            <a href="#"
              ><img
                src="../assets/buy-comics-digital-comics.png"
                alt="Comics Digital"
              />
              <span>DIGITAL COMICS</span>
            </a>
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/buy-comics-merchandise.png"
                alt="Merchandise"
              />
              <span>DC MERCHANDISE</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/buy-comics-subscriptions.png"
                alt="Subscriptions"
              />
              <span>SUBSCRIPTIONS</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img
                src="../assets/buy-comics-shop-locator.png"
                alt="Shop locator"
              />
              <span>COMICS SHOP LOCATOR</span></a
            >
          </li>
          <li>
            <a href="#"
              ><img src="../assets/buy-dc-power-visa.svg" alt="Power Visa" />
              <span>DC POWER VISA</span></a
            >
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "MainTop",
};
</script>

<style lang="scss" scoped>
header {
  background-color: #0282f9;
  padding: 10px;

  ul {
    display: flex;
    align-items: center;
    list-style-type: none;

    a {
      display: flex;
      align-items: center;
      text-decoration: none;
      color: white;
      font-size: 12px;

      img {
        width: 15%;
      }
    }
  }
}
</style>