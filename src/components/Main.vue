<template>
  <main>
      <section id="content">Contenuto!</section>
      <nav>
          <ul>
              <li v-for="link, i in links" :key="i">
                  <img :src="link.img" alt="">
                  <a href="#">{{link.text}}</a>
              </li>
          </ul>
      </nav>
  </main>
</template>

<script>
export default {
  name: 'Main',
  data() {
      return {
          links: [
              {
                  img: "../assets/img/buy-comics-digital-comics.png",
                  text: "DIGITAL COMICS"
              },

              {
                  img: "../assets/img/buy-comics-digital-comics.png",
                  text: "DC MERCHANDISE"
              },

              {
                  img: "../assets/img/buy-comics-digital-comics.png",
                  text: "SUBSCRIPTION"
              },

              {
                  img: "../assets/img/buy-comics-digital-comics.png",
                  text: "COMIC SHOP LOCATOR"
              },

              {
                  img: "../assets/img/buy-comics-digital-comics.png",
                  text: "DC POWER VISA"
              }
          ]
      }
  }
}
</script>

<style scoped lang="scss">
main {
    #content {
        height: 100px;
        background-color: #000;
        color: #fff;
    }
    nav {
        height: 100px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #0182f9;
        li {
            display: inline-block;
            margin: 15px;
            a {
                text-decoration: none;
                color: #fff;
            }
        }
    }
}
</style>