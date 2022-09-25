<template>
  <LazyHydrate when-visible>
    <main>
      <header class="mastheadblog format-webp">
        <div class="container d-flex h-100 align-items-center">
          <div class="mx-auto text-center">
            <h1 class="mx-auto my-0 text-uppercase">Research Posts</h1>
            <h2 class="text-white mx-auto mt-2 mb-5">Follow my articles where I share my personal work, passions and tips for web development.</h2>
          </div>
        </div>
      </header>
      <section class="container">
        <div class="crumbs"><nuxt-link to="/blog/">Blog</nuxt-link>&nbsp;&bull;&nbsp; Research Posts</div>
        <ul>
          <li v-for="article of articles" :key="article.slug">
            <NuxtLink :to="{ name: 'blog-slug', params: { slug: article.slug } }">
              <div>
                <h2>{{ article.title }}</h2>
                <p>by Jerome Heuze</p>
                <p>{{ article.description }}</p>
              </div>
            </NuxtLink>
          </li>
        </ul>
      </section>
      <Footer/>
    </main>
  </LazyHydrate>
</template>

<script>
import Footer from "~/components/footer";
import LazyHydrate from 'vue-lazy-hydration';
export default {
  async asyncData({ $content, params }) {
    const articles = await $content('articles')
        .where({ tags: { $contains: "research" } })
        .sortBy('createdAt', 'asc')
        .fetch()

    return {
      articles
    }
  },
  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('en', options)
    }
  },
  components: {LazyHydrate, Footer}
}
</script>