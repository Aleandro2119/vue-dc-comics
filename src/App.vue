<template>
  <div id="app">
    <Header />
    <HeaderBottom />
    <MainTop />
    <Footer />
    <FooterBottom />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import HeaderBottom from "./components/HeaderBottom.vue";
import MainTop from "./components/MainTop.vue";
import Footer from "./components/Footer.vue";
import FooterBottom from "./components/FooterBottom.vue";

export default {
  name: "App",
  components: {
    Header,
    HeaderBottom,
    MainTop,
    Footer,
    FooterBottom,
  },
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
