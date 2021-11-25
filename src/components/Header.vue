<template>
  <header>
      <img src="../assets/img/dc-logo.png" alt="logo-header">
      <nav>
        <ul>
            <li v-for="link, i in links" :key="i">
                <a href="#">{{link.text}}</a>
            </li>
        </ul>
      </nav>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          links: [
              {
                  text: "CHARACTERS"
              },

              {
                  text: "COMICS"
              },

              {
                  text: "MOVIES"
              },

              {
                  text: "TV"
              },

              {
                  text: "GAMES"
              },

              {
                  text: "COLLECTIBLES"
              },

              {
                  text: "VIDEOS"
              },

              {
                  text: "FANS"
              },

              {
                  text: "NEWS"
              },

              {
                  text: "SHOP"
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">
header {
    display: flex;
    justify-content: center;
    align-items: center;
        img {
            height: 60px;
            margin: 10px 200px 10px 0px;
        }
        li {
            display: inline-block;
            margin: 15px;
            a {
                text-decoration: none;
                color: #000;
            }
            a:hover {
                color: #0182f9;
            }
        }
}
</style>