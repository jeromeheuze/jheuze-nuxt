<template>
  <LazyHydrate when-visible>

    <main>
      <Header/>
      <section class="about-section">
        <div class="container">
          <div class="row">
            <div class="col-xs-12 col-sm-12 col-md-12 col-lg-8 col-lg-offset-2">
              <h2 class="text-white mb-4 text-center">About</h2>
              <p class="text-white-50">Indie game developer, Blender3D, Tangent learning advocate, Web Developer, Front End Developer, Crypto mining and trading enthusiast!</p>
              <p class="text-white-50">Jerome Heuze was born and raised in Paris, France. Having moved to the United States as an exchange student in his teens, he attended high school in Michigan then University in California.</p>
              <p class="text-white-50">Following completion of his studies, Jerome went on to work for 10 years as a Software Engineer in several industries. At present he is doing work for sustainability businesses, Crypto currency companies and mobile games developers.</p>
              <p class="text-white-50">An entrepreneur at heart, Jerome is always looking for ways to educate and entertain, but he is also a budding writer, creating video games and creating beautiful scenes in Blender.</p>
              <p class="text-white-50">In his spare time Jerome enjoys wandering around museums, making and collecting games, building websites, electronics, crypto mining and teaching his daughters about creativity, digital technology and science. He also has a keen interest in astronomy, archery and science fiction entertainment.</p>
              <p class="text-white-50">Jerome is looking forward to the day when space tourism becomes a reality and will allow people to travel throughout the solar system. Maybe one day he will take a vacation on Mars, or in Earth’s orbit.</p>
            </div>
          </div>
        </div>
      </section>
      <section class="projects-section bg-light">
        <div class="container">

          <!-- Featured Project Row -->
          <div class="row align-items-center no-gutters mb-pro">
            <div class="col-xl-6 col-lg-6">
              <img class="img-fluid mb-3 mb-lg-0" src="/img/bg-websites.jpg" alt="websites">
            </div>
            <div class="col-xl-6 col-lg-6">
              <div class="featured-text text-center text-lg-left">
                <h4>Virtual Estates &amp; Digital Investments</h4>
                <p class="text-black-50 mb-0">I own in-game estates as investment:</p>
                <ul style="margin-top: 1rem;">
                  <li><a href="https://www.entropiauniverse.com" target="_blank">Entropia Universe</a> – the Sci-Fi MMORPG, Multi-World, Real Cash Economy Experience.</li>
                  <li><a href="https://app.earth2.io/#profile/85c750d8-93f6-4e71-bc53-1b7a509d7a75" target="_blank">Earth 2</a> - 7.5% promo code - e2japan</li>
                </ul>
              </div>
            </div>
          </div>

          <!-- Project 1 Row -->
          <div class="row justify-content-center no-gutters mb-pro">
            <div class="col-lg-6 mb-3 mb-lg-0">
              <a href="https://heuzeproductions.com" target="_blank"><img class="img-fluid" src="/img/bg-games.jpg" alt="games"></a>
            </div>
            <div class="col-lg-6">
              <div class="featured-text text-center h-100 project">
                <div class="d-flex h-100">
                  <div class="project-text w-100 my-auto text-center text-lg-left">
                    <h4 class="text-white">Indie Video Games Portfolio</h4>
                    <p class="text-black-50">My game projects:</p>
                    <ul style="margin-top: 1rem;">
                      <li><a target="_blank" href="https://heuzeproductions.itch.io/treasure-flip-halloween-edition">Treasure Flip: Halloween Edition</a></li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Project 2 Row -->
          <div class="row justify-content-center no-gutters mb-pro">
            <div class="col-lg-6">
              <a href="https://unsplash.com/@jeromeheuze" target="_blank"><img class="img-fluid" src="/img/demo-image-02.jpg" alt=""></a>
            </div>
            <div class="col-lg-6 order-lg-first">
              <div class="featured-text text-center h-100 project">
                <div class="d-flex h-100">
                  <div class="project-text w-100 my-auto text-center text-lg-right">
                    <h4 class="text-white">Photography</h4>
                    <p class="mb-0 text-white-50"><a target="_blank" href="https://unsplash.com/@jeromeheuze">Download free</a>, beautiful high-quality photos curated by Me.</p>

                  </div>
                </div>
              </div>
            </div>
          </div>

          <!-- Project 3 Row -->
          <div class="row justify-content-center no-gutters mb-pro">
            <div class="col-lg-6">
              <img class="img-fluid" src="/img/bg-mashweb.jpg" alt="">
            </div>
            <div class="col-lg-6 order-lg-first">
              <div class="featured-text text-center h-100 project">
                <div class="d-flex h-100">
                  <div class="project-text w-100 my-auto text-center text-lg-right">
                    <h4 class="text-white">Other Websites I own and maintain:</h4>
                    <ul style="margin-top: 1rem;">
                      <li><a target="_blank" href="https://10kgame.studio">10kgame.studio</a> PHP - HTML/CSS</li>
                      <li><a target="_blank" href="https://academialore.com">academialore.com</a> PHP - HTML/CSS</li>
                      <li><a target="_blank" href="https://bookfairytales.com">bookfairytales.com</a> TBD</li>
                      <li><a target="_blank" href="https://e2.university">e2.university</a> PHP - HTML/CSS</li>
                      <li><a target="_blank" href="https://e2japan.com">e2japan.com</a> TBD</li>
                      <li><a target="_blank" href="https://e2production.com">e2production.com</a> NuxtJS 2.x / Netlify</li>
                      <li><a target="_blank" href="https://entropia.estate">entropia.estate</a> NuxtJS 3.x / Netlify / Supabase</li>
                      <li><a target="_blank" href="https://entropiahub.com">entropiahub.com</a> PHP - HTML/CSS - MySQLi</li>
                      <li><a target="_blank" href="https://foma-asteroid.com">foma-asteroid.com</a> PHP - HTML/CSS</li>
                      <li><a target="_blank" href="https://formly.pro">formly.pro</a> PHP - HTML/CSS - MySQLi</li>
                      <li><a target="_blank" href="https://gddmaker.com">gddmaker.com</a> PHP - HTML/CSS - MySQLi</li>
                      <li><a target="_blank" href="https://geolocationalmetaverse.com">geolocationalmetaverse.com</a> PHP - HTML/CSS</li>
                      <li><a target="_blank" href="https://heuzeproductions.com">heuzeproductions.com</a> PHP - HTML/CSS</li>
                      <li><a target="_blank" href="https://kohibou.com">kohibou.com</a> TBD</li>
                      <li><a target="_blank" href="https://mathk12.tools">mathk12.tools</a> TBD</li>
                      <li><a target="_blank" href="https://openbooktutorials.com">openbooktutorials.com</a> NuxtJS 3.x / Netlify / Blog</li>
                      <li><a target="_blank" href="https://spacescience.degree">spacescience.degree</a> NuxtJS 3.x / Netlify</li>
                      <li><a target="_blank" href="https://sukarei-jewelry.com">sukarei-jewelry.com</a> TBD</li>
                    </ul>
                  </div>
                </div>
              </div>
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