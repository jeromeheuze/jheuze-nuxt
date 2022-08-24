<template>
  <LazyHydrate when-visible>

    <main>
      <Header/>
      <div class="wrapper">
        <h1>Jerome Heuze is coming soon<span class="dot">.</span></h1>
        <p>Indie game developer, Front End Developer, Crypto mining and trading enthusiast!</p>
        <p>Visit my other websites I make and maintain.</p>
        <div class="icons">
          <a href="https://e2production.com"><i class="fa fa-link"></i></a>
          <a href="https://heuzeproductions.com"><i class="fa fa-link"></i></a>
        </div>
      </div>
      <Footer/>
    </main>

  </LazyHydrate>
</template>

<script>
import Header from "~/components/header";
import Footer from "~/components/footer";
import LazyHydrate from 'vue-lazy-hydration';
export default {
  head () {
    return {
      bodyAttrs: {
        class: 'v1'
      },
      title: 'Home',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Indie game developer, Front End Developer, Crypto mining and trading enthusiast!'
        }
      ],
      style: [
      ],
      script: [
      ]
    }
  },
  modules: [],
  components: {LazyHydrate, Footer, Header}
}
</script>