<template>
  <main>
      <section id="content">Contenuto!</section>
      <nav>
          <ul>
              <li v-for="link, i in links" :key="i">
                  <img :src="require(`../assets/img/${link.img}`)" alt="">
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
                  img: "buy-comics-digital-comics.png",
                  text: "DIGITAL COMICS"
              },

              {
                  img: "buy-comics-merchandise.png",
                  text: "DC MERCHANDISE"
              },

              {
                  img: "buy-comics-shop-locator.png",
                  text: "SUBSCRIPTION"
              },

              {
                  img: "buy-comics-subscriptions.png",
                  text: "COMIC SHOP LOCATOR"
              },

              {
                  img: "buy-dc-power-visa.svg",
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
            img {
                height: 40px;
                margin-right: 10px;
            }
            a {
                text-decoration: none;
                color: #fff;
            }
        }
    }
}
</style>