<template>
  <header>
    <div class="container">
      <div>
        <img src="../assets/dc-logo.png" alt="Logo" />
      </div>
      <nav>
        <ul>
          <li v-for="(link, index) in links" :key="index">
            <a href="#">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      links: [
        { text: "CHARACTERS", url: "#" },
        { text: "COMICS", url: "#" },
        { text: "MOVIES", url: "#" },
        { text: "TV", url: "#" },
        { text: "GAMES", url: "#" },
        { text: "COLLECTIBLES", url: "#" },
        { text: "VIDEOS", url: "#" },
        { text: "FANS", url: "#" },
        { text: "NEWS", url: "#" },
        { text: "SHOP", url: "#" },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
header {
  background-color: white;
  padding: 10px;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    ul {
      display: flex;
      list-style-type: none;

      li {
        padding: 10px;

        a {
          text-decoration: none;
          color: #303030;
          font-size: 12px;
          font-weight: bold;
        }
      }
    }
  }
}
</style>