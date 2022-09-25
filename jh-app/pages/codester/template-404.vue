<template>
  <LazyHydrate when-visible>
    <main>
      <div class="section404">
        404
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
        class: 'v1'
      },
      title: 'Template 404 from Codester',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Checkout my templates, web tools, and templates on Codester marketplace.'
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

<style lang="scss" scoped>
body, html {
  padding: 0;
  margin: 0;
}
main {
  background: url("/img/codester/purple-abstract.jpg") center center no-repeat #111;
  background-size: cover;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-content: center;
  align-items: center;
}
</style>