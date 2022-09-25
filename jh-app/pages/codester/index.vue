<template>
  <LazyHydrate when-visible>

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
      title: 'My work on Codester marketplace',
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