<template>
  <LazyHydrate when-visible>
    <main>
      <header class="mastheadblog posts format-webp">
        <div class="container d-flex h-100 align-items-center">
          <div class="mx-auto text-center">
            <h1 class="mx-auto my-0 text-uppercase">{{ article.title }}</h1>
            <h2 class="text-white mx-auto mt-2 mb-5">{{ article.description }}</h2>
            <p>Article last updated: {{ formatDate(article.updatedAt) }}</p>
          </div>
        </div>
      </header>
      <section class="container">
        <div class="crumbs"><nuxt-link to="/blog/">Blog</nuxt-link>&nbsp;&bull;&nbsp; {{ article.title }}</div>
      <article>
        <span class="tags" v-for="tag in article.tags" :key="tag">

            <span class="tag">
              {{ tag }}
            </span>
          
        </span>
        <nuxt-content class="nuxt-content" :document="article" />
      </article>
      <prev-next :prev="prev" :next="next" />
      </section>
      <Footer/>
    </main>
  </LazyHydrate>
</template>

<script>
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
        //{hid: 'highlight', src: '//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.6.0/styles/default.min.css'}
      ],
      script: [
        //{src: '//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.6.0/highlight.min.js'}
      ]
    }
  },
  methods: {
    formatDate(date) {
      const options = { year: 'numeric', month: 'long', day: 'numeric' }
      return new Date(date).toLocaleDateString('en', options)
    }
  },
  async asyncData({ $content, params }) {
    const article = await $content('blog', params.slug).fetch()

    const [prev, next] = await $content('blog')
        .only(['title', 'slug'])
        .sortBy('createdAt', 'asc')
        .surround(params.slug)
        .fetch()

    return { article, prev, next }
  },
  modules: [],
  components: {LazyHydrate, Footer}
}
</script>

<style scoped>
.nuxt-content h2 {
  font-weight: bold;
  font-size: 28px;
}
.nuxt-content h3 {
  font-weight: bold;
  font-size: 22px;
}
.nuxt-content p {
  margin-bottom: 20px;
}
/* Code blocks */
pre {
  padding: 1em;
  margin: .5em 0;
  overflow: auto;
  background: #f5f2f0;
}

code,
pre {
  color: black;
  background: none;
  text-shadow: 0 1px white;
  font-family: Consolas, Monaco, 'Andale Mono', 'Ubuntu Mono', monospace;
  font-size: 1em;
  text-align: left;
  white-space: pre;
  word-spacing: normal;
  word-break: normal;
  word-wrap: normal;
  line-height: 1.5;

  -moz-tab-size: 4;
  -o-tab-size: 4;
  tab-size: 4;

  -webkit-hyphens: none;
  hyphens: none;
}
</style>