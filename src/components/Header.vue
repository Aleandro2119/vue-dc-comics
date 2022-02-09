<template>
  <header>
    <div class="container">
      <div>
        <img src="../assets/dc-logo.png" alt="Logo" />
      </div>
      <nav>
        <ul>
          <li><a href="#">CHARACTERS</a></li>
          <li><a href="#">COMICS</a></li>
          <li><a href="#">MOVIES</a></li>
          <li><a href="#">TV</a></li>
          <li><a href="#">GAMES</a></li>
          <li><a href="#">COLLECTIBLES</a></li>
          <li><a href="#">VIDEOS</a></li>
          <li><a href="#">FANS</a></li>
          <li><a href="#">NEWS</a></li>
          <li><a href="#">SHOP</a></li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
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