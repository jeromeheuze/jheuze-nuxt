<template>
  <LazyHydrate when-visible>
    <main>
        <header class="mastheadblog format-webp">
          <div class="container d-flex h-100 align-items-center">
            <div class="mx-auto text-center">
              <h1 class="mx-auto my-0 text-uppercase">Blog Posts</h1>
              <h2 class="text-white mx-auto mt-2 mb-5">Follow my articles where I share my personal work, passions and tips for web development.</h2>
            </div>
          </div>
        </header>
        <section class="container">
          <div class="crumbs"><nuxt-link to="/">Home</nuxt-link>&nbsp;&bull;&nbsp; Blog</div>

          <ul class="blog-list">
            <li v-for="article of articles" :key="article.slug">

                <div>
                  <h2><NuxtLink :to="{ name: 'blog-slug', params: { slug: article.slug } }">{{ article.title }}</NuxtLink></h2>
                  <p>by Jerome Heuze</p>
                  <p>{{ article.description }}</p>
                </div>

            </li>
          </ul>
        </section>
      <Footer/>
    </main>
  </LazyHydrate>
</template>

<script>
import AppSearchInput from "~/components/AppSearchInput";
import Footer from "~/components/footer";
import LazyHydrate from 'vue-lazy-hydration';
export default {
  head () {
    return {
      bodyAttrs: {
        class: 'v1'
      },
      title: 'Blog',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Follow my blog where I share my personal work, passions and tips for web development.'
        }
      ],
      style: [
      ],
      script: [
      ]
    }
  },
  async asyncData({ $content, params }) {
    const articles = await $content('blog')
        .only(['title', 'description', 'slug'])
        .sortBy('createdAt', 'asc')
        .fetch()

    return {
      articles
    }
  },
  modules: [],
  components: {LazyHydrate, Footer, AppSearchInput}
}
</script>