<template>
  <LazyHydrate when-visible>
    <main class="pagenotfound">
      <div class="section404">
        <h1>4<span></span>4</h1>
        <h2>Oh no! That page can't be found.</h2>
        <p>It looks like nothing was found at this location.</p>
        <a href="/">Go back</a>
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
        class: 'Codester'
      },
      title: 'NuxtJS - 404 Page - abstract',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'NuxtJS - 404 Page - abstract - from Codester.com'
        }
      ],
      style: [
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
.pagenotfound {
  background: url("/img/codester/purple-abstract.jpg") center center no-repeat #111;
  background-size: cover;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
  text-align: center;
}
.pagenotfound h1 {
  font-size: 10rem;
  line-height: 10rem;
}
.pagenotfound h1 span {
  background: url(/svg/icon-x-circle.svg) center center no-repeat transparent;
  background-size: contain;
  display: inline-block;
  width: 13rem;
  height: 10rem;
}
.pagenotfound p {
  margin-bottom: 1rem;
}
.pagenotfound a {
  font-size: 1.4rem;
  color: #fff;
}
/* Portrait */
@media only screen
and (min-device-width: 320px)
and (max-device-width: 480px)
and (-webkit-min-device-pixel-ratio: 2)
and (orientation: portrait) {
  .pagenotfound h1 span {
    width: 10rem;
  }
}
</style>