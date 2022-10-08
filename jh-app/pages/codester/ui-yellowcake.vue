<template>
  <LazyHydrate when-visible>
    <main class="yellowcake">

      <div class="theme">
        <p class="h1">YellowCake <span style="color:#d9f4c7;">UI</span> Theme</p>
        <div>
          <p>Color used <span>#F8FA90</span>, <span>#F4EF88</span>, <span>#D9F4C7</span>, <span>#9DCDC0</span>, <span>#AC9969</span></p>
          <h1>H1 Header</h1>
          <h2>H2 Header</h2>
          <h3>H3 Header</h3>
          <h4>H4 Header</h4>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          <ul>
            <li>Lorem ipsum dolor sit amet, consectetur adipiscing.</li>
            <li>Lorem ipsum dolor sit amet, consectetur adipiscing.</li>
            <li>Lorem ipsum dolor sit amet, consectetur adipiscing.</li>
            <li>Lorem ipsum dolor sit amet, consectetur adipiscing.</li>
            <li>Lorem ipsum dolor sit amet, consectetur adipiscing.</li>
          </ul>

          <div style="margin: 3rem 0;">
            <p>Primary</p>
            <a href="#" class="btn yc-primary">Send Message</a>
          </div>
          <div style="margin: 3rem 0;">
            <p>Secondary</p>
            <a href="#" class="btn yc-secondary">Send Message</a>
          </div>
          <div style="margin: 3rem 0;">
            <p>Primary Outline</p>
            <a href="#" class="btn yc-primary-outline">Send Message</a>
          </div>
          <div style="margin: 3rem 0;">
            <p>Secondary Outline</p>
            <a href="#" class="btn yc-secondary-outline">Send Message</a>
          </div>

        </div>
      </div>

    </main>
  </LazyHydrate>
</template>

<script>
import LazyHydrate from 'vue-lazy-hydration';
export default {
  head () {
    return {
      bodyAttrs: {
        class: 'yellowcake'
      },
      title: 'YellowCake UI Theme - UI kit for sale',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'YellowCake UI Theme - purchase UI kit on Codester.com'
        }
      ],
      style: [
        {hid: 'gfont', href: 'https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;800&display=swap', rel: 'stylesheet'}
      ],
      script: [
      ]
    }
  },
  modules: [],
  components: {LazyHydrate}
}
</script>

<style lang="css" scoped>
body, html {
  padding: 0;
  margin: 0;
}
main {
  display: flex;
  width: 1024px;
  margin: 5rem auto;
  justify-content: center;
  align-content: center;
  align-items: center;
}
.yellowcake {
  font-family: 'Montserrat', sans-serif;
  font-size: 1rem;
  font-weight: 400;
}
.yellowcake h1, .yellowcake .h1 {
  font-size: 4rem;
  line-height: 4.3rem;
  font-weight: 800;
}
.yellowcake h2, .yellowcake .h2 {
  font-size: 3rem;
  line-height: 3.3rem;
  font-weight: 800;
}
.yellowcake h3, .yellowcake .h3 {
  font-size: 2.5rem;
  line-height: 2.8rem;
  font-weight: 800;
}
.yellowcake h4, .yellowcake .h4 {
  font-size: 1.5rem;
  line-height: 1.8rem;
  font-weight: 800;
}
.yellowcake p {
  font-size: 1rem;
  line-height: 1.4rem;
  margin-bottom: 1rem;
}
.yellowcake ul {
  margin: 3rem 0 3rem 2rem;
  list-style-type: disc;
}
.yellowcake ul li {
  margin-bottom: .75rem;
}
.yellowcake .btn {
  text-transform: uppercase;
  color: #111;
}
.yellowcake .btn:hover {
  color: #000;
}
.yellowcake .btn.yc-primary {
  background: #F8FA90;
}
.yellowcake .btn.yc-primary:hover {
  background: #F4EF88;
}
.yellowcake .btn.yc-secondary {
  background: #D9F4C7;
}
.yellowcake .btn.yc-secondary:hover {
  background: #9DCDC0;
}
.yellowcake .btn.yc-primary-outline {
  border-color: #AC9969;
}
.yellowcake .btn.yc-primary-outline:hover {
  background: #AC9969;
  color: #fff;
}
.yellowcake .btn.yc-secondary-outline {
  border-color: #9DCDC0;
}
.yellowcake .btn.yc-secondary-outline:hover {
  background: #9DCDC0;
}
/* Portrait */
@media only screen
and (min-device-width: 320px)
and (max-device-width: 480px)
and (-webkit-min-device-pixel-ratio: 2)
and (orientation: portrait) {

}
</style>