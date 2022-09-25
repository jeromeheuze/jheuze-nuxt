---
title: Fixing NuxtJS 2.x with Supabase
description: Learning how to fix supabase project while using NuxtJS 2.x.
tags:
 - nuxtjs
 - netlify
 - supabase
---

It took me a few days to fix this challenging issue I had with my NuxtJS project where suddenly it would not compile in Netlify. My website was stuck and finally here was my solution.

Here my dependencies for my **package.json** file:

```
"dependencies": {
"@nuxt/content": "^1.14.0",
"@nuxtjs/axios": "^5.13.6",
"@nuxtjs/lunr-module": "^0.3.2",
"@nuxtjs/redirect-module": "^0.3.1",
"@nuxtjs/robots": "^2.5.0",
"@nuxtjs/sitemap": "^2.4.0",
"chart.js": "^3.7.1",
"core-js": "^3.15.1",
"dotenv": "^10.0.0",
"hchs-vue-charts": "^1.2.8",
"netlify-cli": "^8.19.3",
"nuxt": "^2.15.7",
"nuxt-canonical": "^1.0.6",
"nuxt-social-meta": "^1.0.0",
"v-clipboard": "^2.2.3",
"vue": "^2.7.8",
"vue-gtag": "^1.16.1",
"vue-lazy-hydration": "^2.0.0-beta.4",
"vue-server-renderer": "^2.7.8",
"vue-supabase": "^2.3.0"
}
```

The important versions are:
- "nuxt": "^2.15.7",
- "vue": "^2.7.8",
- "vue-server-renderer": "^2.7.8",
- "vue-supabase": "^2.3.0"

Then make a js file inside your **/plugins/** folder called **supabase.js**

```
import Vue from "vue"
import VueSupabase from "vue-supabase";
Vue.use(VueSupabase, {
supabaseUrl: "https://xxxxx.supabase.co",
supabaseKey: "xxxx-xxxx",
supabaseOptions: {},
});
```

Then lets import the plug inside your **nuxt.config.js**

```
// Plugins to run before rendering page: https://go.nuxtjs.dev/config-plugins
plugins: [
{ src: '~/plugins/supabase.js' }
]
```

Hope it helps someone because I could not find any detailed fixes. Enjoy!