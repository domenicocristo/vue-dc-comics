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
  date() {
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

</style>