<template>
  <footer>
      <nav>
          <section>
              <h3>DC COMICS</h3>
              <ul>
                  <li v-for="link, i in dcComics" :key="i">
                      <a href="#">{{link.text}}</a>
                  </li>
              </ul>
          </section>

          <section>
              <h3>SHOP</h3>
              <ul>
                  <li v-for="link, i in shop" :key="i">
                      <a href="#">{{link.text}}</a>
                  </li>
              </ul>
          </section>

          <section>
              <h3>DC</h3>
              <ul>
                  <li v-for="link, i in dc" :key="i">
                      <a href="#">{{link.text}}</a>
                  </li>
              </ul>
          </section>

          <section>
              <h3>SITES</h3>
              <ul>
                  <li v-for="link, i in sites" :key="i">
                      <a href="#">{{link.text}}</a>
                  </li>
              </ul>
          </section>
      </nav>
      <section id="social">
          <button>SIGN-UP NOW!</button>
          <h4>FOLLOW US</h4>
          <img src="../assets/img/footer-facebook.png" alt="social">
          <img src="../assets/img/footer-twitter.png" alt="social">
          <img src="../assets/img/footer-youtube.png" alt="social">
          <img src="../assets/img/footer-pinterest.png" alt="social">
          <img src="../assets/img/footer-periscope.png" alt="social">
      </section>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
  data() {
      return {
          dcComics: [
              {
                  text: "Characters"
              },

              {
                  text: "Comics"
              },

              {
                  text: "Movies"
              },

              {
                  text: "Tv"
              },

              {
                  text: "Games"
              },

              {
                  text: "Videos"
              },

              {
                  text: "News"
              },
          ],
          shop: [
              {
                  text: "Shop DC"
              },

              {
                  text: "Shop DC Collectibles"
              }
          ],
          dc: [
              {
                  text: "Terms Of Use"
              },

              {
                  text: "Privacy policy (new)"
              },

              {
                  text: "Ad Choices"
              },

              {
                  text: "Advertising"
              },

              {
                  text: "Jobs"
              },

              {
                  text: "Subscriptions"
              },

              {
                  text: "Talent Workshops"
              },

              {
                  text: "CPSC Certificates"
              },

              {
                  text: "Ratings"
              },

              {
                  text: "Shop Help"
              },

              {
                  text: "Contact Us"
              }
          ],
          sites: [
              {
                  text: "DC"
              },

              {
                  text: "MAD Magazine"
              },

              {
                  text: "DC Kids"
              },

              {
                  text: "DC Universe"
              },

              {
                  text: "DC Power Visa"
              },
          ]
      }
  }
}
</script>

<style scoped lang="scss">
footer {
    nav {
        height: 350px;
        background-image: url(../assets/img/footer-bg.jpg);
        section {
            display: inline-block;
            h3 {
                color: #fff;
            }
            ul {
                list-style-type: none;
                li {
                    a {
                        text-decoration: none;
                        color: #8d8c8c;
                    }
                }
            }
        }
    }
}

#social {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #303030;
    button {
        height: 50px;
        display: inline-block;
        margin-right: 200px;
        padding: 10px;
        background-color: #303030;
        border: none;
        border: 2px solid #0182f9;
        color: #fff;
    }
    h4 {
        display: inline-block;
        margin-right: 20px;
        font-size: 20px;
        color: #0082f8;
    }
    img {
        height: 40px;
        margin: 5px;
    }
}
</style>