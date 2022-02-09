<template>
  <footer>
    <div class="container">
      <a href="#">SIGN-UP NOW!</a>

      <div class="social-box">
        <h4>FOLLOW US</h4>
        <img src="../assets/footer-facebook.png" alt="Facebook" />
        <img src="../assets/footer-twitter.png" alt="Twitter" />
        <img src="../assets/footer-youtube.png" alt="YouTube" />
        <img src="../assets/footer-pinterest.png" alt="Pinterest" />
        <img src="../assets/footer-periscope.png" alt="Periscope" />
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style lang="scss" scoped>
footer {
  background-color: #303030;
  padding: 30px;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    a {
      color: white;
      font-size: 14px;
      padding: 10px;
      border: 2px solid #0282d9;
      text-decoration: none;
    }

    .social-box {
      display: flex;
      align-items: center;
    }

    h4 {
      color: #0282d9;
      padding-right: 10px;
      font-size: 18px;
    }

    img {
      padding: 0 10px;
      cursor: pointer;
    }
  }
}
</style>