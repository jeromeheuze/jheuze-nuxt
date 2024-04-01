<template>
  <LazyHydrate when-visible>

    <main>
      <Header/>
      <section class="about-section">
        <div class="container">
          <div class="row">
            <div class="col-xs-12 col-sm-12 col-md-12 col-lg-8 col-lg-offset-2">
              <h2 class="text-white mb-4 text-center">Wallet</h2>
              <p class="text-white-50">YTN: YcrrohT2pkqhPTSyaqFjKfoERZgMLyLn9w</p>
              <p class="text-white-50">./minerd -a yespowerR16 -o stratum+tcp://cpu-pool.com:63368 -u YcrrohT2pkqhPTSyaqFjKfoERZgMLyLn9w -p x -t 4</p>
            </div>
          </div>
        </div>
      </section>
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
      title: 'Wallet',
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