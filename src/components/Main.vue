<template>
  <main>
      <section id="jumbotron">
          <button>
              <h2>CORRENT SERIES</h2>
          </button>
      </section>
      <section id="content">
          <Series/>
      </section>
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
import Series from './Series.vue';

export default {
  name: 'Main',
  components: {
    Series
  },
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
    #jumbotron {
        height: 300px;
        background-image: url(../assets/img/jumbotron.jpg);
    }
        button {
            padding: 10px 20px;
            background-color: #0182f9;
            border: none;
            color: #fff;
            cursor: pointer;
            margin: 20% 100px;
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
                vertical-align: middle;
            }
            a {
                text-decoration: none;
                color: #fff;
            }
        }
    }
}
</style>