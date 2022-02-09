<template>
  <div id="app">
    <Header />
    <HeaderBottom />
    <MainTop />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import HeaderBottom from "./components/HeaderBottom.vue";
import MainTop from "./components/MainTop.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    HeaderBottom,
    MainTop,
    Footer,
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
