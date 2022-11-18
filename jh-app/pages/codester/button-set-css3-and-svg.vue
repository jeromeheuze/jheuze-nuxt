<template>
  <LazyHydrate when-visible>
    <main class="btnset">

      <div class="theme">
        <p class="h1">Button Set - CSS3 <span style="color:#d9f4c7;">and</span> SVG</p>

        <div style="display: flex;justify-content: center;align-items:center;margin-top: 4rem;" v-for="icon in this.btnArr" :key="icon.index">
          <div style="margin: 1rem;"><h2 style="text-align: left;">Icon name: <strong>{{ icon }}</strong></h2></div>
          <div style="margin: 1rem;">
            <a href="#" :class="'btn bss-primary bss-icon bss-icon-left '+icon"><em></em>  {{ icon }}</a>
          </div>
          <div style="margin: 1rem;">
            <a href="#" :class="'btn bss-primary bss-icon '+icon"><em></em></a>
          </div>
          <div style="margin: 1rem;">
            <a href="#" :class="'btn bss-primary bss-icon bss-icon-right '+icon"> {{ icon }} <em></em></a>
          </div>
        </div>

      </div>

    </main>
  </LazyHydrate>
</template>

<script>
import LazyHydrate from 'vue-lazy-hydration';
export default {
  data() {
    return {
      btnArr: [
        'icon-announcement',
        'icon-archive',
        'icon-arrow-down',
        'icon-arrow-left',
        'icon-arrow-right',
        'icon-arrow-up',
        'icon-at-symbol',
        'icon-book',
        'icon-bookmark',
        'icon-briefcase',
        'icon-browser',
        'icon-building',
        'icon-calendar',
        'icon-call',
        'icon-call-incoming',
        'icon-call-outgoing',
        'icon-camera',
        'icon-cart',
        'icon-chat',
        'icon-check-circle',
        'icon-chevron-down',
        'icon-chevron-left',
        'icon-chevron-right',
        'icon-chevron-up',
        'icon-clip',
        'icon-clipboard',
        'icon-clock',
        'icon-code',
        'icon-cog',
        'icon-comment',
        'icon-compass',
        'icon-currency-dollar',
        'icon-dashboard',
        'icon-desktop',
        'icon-discount',
        'icon-download',
        'icon-duplicate',
        'icon-edit',
        'icon-emotion-happy',
        'icon-emotion-sad',
        'icon-exclamation',
        'icon-external-link',
        'icon-file',
        'icon-file-blank',
        'icon-file-minus',
        'icon-file-plus',
        'icon-film',
        'icon-filter',
        'icon-flag',
        'icon-folder',
        'icon-folder-minus',
        'icon-folder-plus',
        'icon-globe',
        'icon-graph-bar',
        'icon-grid',
        'icon-group',
        'icon-hashtag',
        'icon-heart',
        'icon-help',
        'icon-home',
        'icon-image',
        'icon-inbox',
        'icon-information',
        'icon-key',
        'icon-link',
        'icon-location',
        'icon-lock-closed',
        'icon-lock-open',
        'icon-mail',
        'icon-map',
        'icon-menu',
        'icon-microphone',
        'icon-minus',
        'icon-minus-circle',
        'icon-minus-square',
        'icon-mobile',
        'icon-moon',
        'icon-more-horiz',
        'icon-music',
        'icon-news',
        'icon-notification',
        'icon-plus',
        'icon-plus-circle',
        'icon-plus-square',
        'icon-print',
        'icon-puzzle',
        'icon-refresh',
        'icon-repeat',
        'icon-rocket',
        'icon-search',
        'icon-server',
        'icon-speaker',
        'icon-star',
        'icon-store',
        'icon-tablet',
        'icon-tag',
        'icon-thumb-down',
        'icon-thumb-up',
        'icon-trash',
        'icon-trending-down',
        'icon-trending-up',
        'icon-trophy',
        'icon-upload',
        'icon-user',
        'icon-user-check',
        'icon-user-minus',
        'icon-user-plus',
        'icon-video',
        'icon-view',
        'icon-x',
        'icon-x-circle',
        'icon-x-square',
        'icon-zoom-in',
        'icon-zoom-out'
      ]
    }
  },
  head () {
    return {
      bodyAttrs: {
        class: 'btnset'
      },
      title: 'Button Set - CSS3 and SVG for sale',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'Button Set - CSS3 and SVG on Codester.com'
        }
      ],
      style: [
        {hid: 'gfont', href: 'https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;800&display=swap', rel: 'stylesheet'}
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
strong {
  font-weight: bold;
}
main {
  display: flex;
  width: 1024px;
  margin: 5rem auto;
  justify-content: center;
  align-content: center;
  align-items: center;
}
.btnset .h1 {
  font-family: 'Montserrat', sans-serif;
  font-size: 4rem;
  line-height: 4.3rem;
  font-weight: 800;
}
.btnset {
  font-family: 'Montserrat', sans-serif;
  font-size: 1rem;
  font-weight: 400;
}

.btnset .btn {
  text-transform: uppercase;
  color: #000;
  border: 1px solid transparent;
  border-radius: 7px;
}
.btnset .btn.bss-primary {
  background: #f5f5f5;
  border: 1px solid #f5f5f5;
}
.btnset .btn.bss-primary:hover {
  background: #fff;
  border: 1px solid #0453F4;
  color: #0453F4;
}
.btnset .btn.bss-primary:active {
  background: #fff;
  border: 1px solid #0453F4;
  color: #0453F4;
}
/* ICONS */
.btn.bss-icon {
  display: flex;
  justify-content: center;
}
.btn.bss-icon.bss-icon-left em {
  margin-right: 7px;
}
.btn.bss-icon.bss-icon-right em {
  margin-left: 7px;
}
.btn.bss-icon em {
  width: 10px;
  height: 10px;
  display: inline-block;
  padding: 7px;
}
/* icon list */
.btn.icon-announcement em {
  background: url("/icons-svg/icon-announcement.svg") center center no-repeat;
}
.btn.icon-archive em {
  background: url("/icons-svg/icon-archive.svg") center center no-repeat;
}
.btn.icon-arrow-down em {
  background: url("/icons-svg/icon-arrow-down.svg") center center no-repeat;
}
.btn.icon-arrow-left em {
  background: url("/icons-svg/icon-arrow-left.svg") center center no-repeat;
}
.btn.icon-arrow-right em {
  background: url("/icons-svg/icon-arrow-right.svg") center center no-repeat;
}
.btn.icon-arrow-up em {
  background: url("/icons-svg/icon-arrow-up.svg") center center no-repeat;
}
.btn.icon-at-symbol em {
  background: url("/icons-svg/icon-at-symbol.svg") center center no-repeat;
}
.btn.icon-book em {
  background: url("/icons-svg/icon-book.svg") center center no-repeat;
}
.btn.icon-bookmark em {
  background: url("/icons-svg/icon-bookmark.svg") center center no-repeat;
}
.btn.icon-briefcase em {
  background: url("/icons-svg/icon-briefcase.svg") center center no-repeat;
}
.btn.icon-browser em {
  background: url("/icons-svg/icon-browser.svg") center center no-repeat;
}
.btn.icon-building em {
  background: url("/icons-svg/icon-building.svg") center center no-repeat;
}
.btn.icon-calendar em {
  background: url("/icons-svg/icon-calendar.svg") center center no-repeat;
}
.btn.icon-call em {
  background: url("/icons-svg/icon-call.svg") center center no-repeat;
}
.btn.icon-call-incoming em {
  background: url("/icons-svg/icon-call-incoming.svg") center center no-repeat;
}
.btn.icon-call-outgoing em {
  background: url("/icons-svg/icon-call-outgoing.svg") center center no-repeat;
}
.btn.icon-camera em {
  background: url("/icons-svg/icon-camera.svg") center center no-repeat;
}
.btn.icon-cart em {
  background: url("/icons-svg/icon-cart.svg") center center no-repeat;
}
.btn.icon-chat em {
  background: url("/icons-svg/icon-chat.svg") center center no-repeat;
}
.btn.icon-check-circle em {
  background: url("/icons-svg/icon-check-circle.svg") center center no-repeat;
}
.btn.icon-chevron-down em {
  background: url("/icons-svg/icon-chevron-down.svg") center center no-repeat;
}
.btn.icon-chevron-left em {
  background: url("/icons-svg/icon-chevron-left.svg") center center no-repeat;
}
.btn.icon-chevron-right em {
  background: url("/icons-svg/icon-chevron-right.svg") center center no-repeat;
}
.btn.icon-chevron-up em {
  background: url("/icons-svg/icon-chevron-up.svg") center center no-repeat;
}
.btn.icon-clip em {
  background: url("/icons-svg/icon-clip.svg") center center no-repeat;
}
.btn.icon-clipboard em {
  background: url("/icons-svg/icon-clipboard.svg") center center no-repeat;
}
.btn.icon-clock em {
  background: url("/icons-svg/icon-clock.svg") center center no-repeat;
}
.btn.icon-code em {
  background: url("/icons-svg/icon-code.svg") center center no-repeat;
}
.btn.icon-cog em {
  background: url("/icons-svg/icon-cog.svg") center center no-repeat;
}
.btn.icon-comment em {
  background: url("/icons-svg/icon-comment.svg") center center no-repeat;
}
.btn.icon-compass em {
  background: url("/icons-svg/icon-compass.svg") center center no-repeat;
}
.btn.icon-currency-dollar em {
  background: url("/icons-svg/icon-currency-dollar.svg") center center no-repeat;
}
.btn.icon-dashboard em {
  background: url("/icons-svg/icon-dashboard.svg") center center no-repeat;
}
.btn.icon-desktop em {
  background: url("/icons-svg/icon-desktop.svg") center center no-repeat;
}
.btn.icon-discount em {
  background: url("/icons-svg/icon-discount.svg") center center no-repeat;
}
.btn.icon-download em {
  background: url("/icons-svg/icon-download.svg") center center no-repeat;
}
.btn.icon-duplicate em {
  background: url("/icons-svg/icon-duplicate.svg") center center no-repeat;
}
.btn.icon-edit em {
  background: url("/icons-svg/icon-edit.svg") center center no-repeat;
}
.btn.icon-emotion-happy em {
  background: url("/icons-svg/icon-emotion-happy.svg") center center no-repeat;
}
.btn.icon-emotion-sad em {
  background: url("/icons-svg/icon-emotion-sad.svg") center center no-repeat;
}
.btn.icon-exclamation em {
  background: url("/icons-svg/icon-exclamation.svg") center center no-repeat;
}
.btn.icon-external-link em {
  background: url("/icons-svg/icon-external-link.svg") center center no-repeat;
}
.btn.icon-file em {
  background: url("/icons-svg/icon-file.svg") center center no-repeat;
}
.btn.icon-file-blank em {
  background: url("/icons-svg/icon-file-blank.svg") center center no-repeat;
}
.btn.icon-file-minus em {
  background: url("/icons-svg/icon-file-minus.svg") center center no-repeat;
}
.btn.icon-file-plus em {
  background: url("/icons-svg/icon-file-plus.svg") center center no-repeat;
}
.btn.icon-film em {
  background: url("/icons-svg/icon-film.svg") center center no-repeat;
}
.btn.icon-filter em {
  background: url("/icons-svg/icon-filter.svg") center center no-repeat;
}
.btn.icon-flag em {
  background: url("/icons-svg/icon-flag.svg") center center no-repeat;
}
.btn.icon-folder em {
  background: url("/icons-svg/icon-folder.svg") center center no-repeat;
}
.btn.icon-folder-minus em {
  background: url("/icons-svg/icon-folder-minus.svg") center center no-repeat;
}
.btn.icon-folder-plus em {
  background: url("/icons-svg/icon-folder-plus.svg") center center no-repeat;
}
.btn.icon-globe em {
  background: url("/icons-svg/icon-globe.svg") center center no-repeat;
}
.btn.icon-graph-bar em {
  background: url("/icons-svg/icon-graph-bar.svg") center center no-repeat;
}
.btn.icon-grid em {
  background: url("/icons-svg/icon-grid.svg") center center no-repeat;
}
.btn.icon-group em {
  background: url("/icons-svg/icon-group.svg") center center no-repeat;
}
.btn.icon-hashtag em {
  background: url("/icons-svg/icon-hashtag.svg") center center no-repeat;
}
.btn.icon-heart em {
  background: url("/icons-svg/icon-heart.svg") center center no-repeat;
}
.btn.icon-help em {
  background: url("/icons-svg/icon-help.svg") center center no-repeat;
}
.btn.icon-home em {
  background: url("/icons-svg/icon-home.svg") center center no-repeat;
}
.btn.icon-image em {
  background: url("/icons-svg/icon-image.svg") center center no-repeat;
}
.btn.icon-inbox em {
  background: url("/icons-svg/icon-inbox.svg") center center no-repeat;
}
.btn.icon-information em {
  background: url("/icons-svg/icon-information.svg") center center no-repeat;
}
.btn.icon-key em {
  background: url("/icons-svg/icon-key.svg") center center no-repeat;
}
.btn.icon-link em {
  background: url("/icons-svg/icon-link.svg") center center no-repeat;
}
.btn.icon-location em {
  background: url("/icons-svg/icon-location.svg") center center no-repeat;
}
.btn.icon-lock-closed em {
  background: url("/icons-svg/icon-lock-closed.svg") center center no-repeat;
}
.btn.icon-lock-open em {
  background: url("/icons-svg/icon-lock-open.svg") center center no-repeat;
}
.btn.icon-mail em {
  background: url("/icons-svg/icon-mail.svg") center center no-repeat;
}
.btn.icon-map em {
  background: url("/icons-svg/icon-map.svg") center center no-repeat;
}
.btn.icon-menu em {
  background: url("/icons-svg/icon-menu.svg") center center no-repeat;
}
.btn.icon-microphone em {
  background: url("/icons-svg/icon-microphone.svg") center center no-repeat;
}
.btn.icon-minus em {
  background: url("/icons-svg/icon-minus.svg") center center no-repeat;
}
.btn.icon-minus-circle em {
  background: url("/icons-svg/icon-minus-circle.svg") center center no-repeat;
}
.btn.icon-minus-square em {
  background: url("/icons-svg/icon-minus-square.svg") center center no-repeat;
}
.btn.icon-mobile em {
  background: url("/icons-svg/icon-mobile.svg") center center no-repeat;
}
.btn.icon-moon em {
  background: url("/icons-svg/icon-moon.svg") center center no-repeat;
}
.btn.icon-more-horiz em {
  background: url("/icons-svg/icon-more-horiz.svg") center center no-repeat;
}
.btn.icon-music em {
  background: url("/icons-svg/icon-music.svg") center center no-repeat;
}
.btn.icon-news em {
  background: url("/icons-svg/icon-news.svg") center center no-repeat;
}
.btn.icon-notification em {
  background: url("/icons-svg/icon-notification.svg") center center no-repeat;
}
.btn.icon-plus em {
  background: url("/icons-svg/icon-plus.svg") center center no-repeat;
}
.btn.icon-plus-circle em {
  background: url("/icons-svg/icon-plus-circle.svg") center center no-repeat;
}
.btn.icon-plus-square em {
  background: url("/icons-svg/icon-plus-square.svg") center center no-repeat;
}
.btn.icon-print em {
  background: url("/icons-svg/icon-print.svg") center center no-repeat;
}
.btn.icon-puzzle em {
  background: url("/icons-svg/icon-puzzle.svg") center center no-repeat;
}
.btn.icon-refresh em {
  background: url("/icons-svg/icon-refresh.svg") center center no-repeat;
}
.btn.icon-repeat em {
  background: url("/icons-svg/icon-repeat.svg") center center no-repeat;
}
.btn.icon-rocket em {
  background: url("/icons-svg/icon-rocket.svg") center center no-repeat;
}
.btn.icon-search em {
  background: url("/icons-svg/icon-search.svg") center center no-repeat;
}
.btn.icon-server em {
  background: url("/icons-svg/icon-server.svg") center center no-repeat;
}
.btn.icon-speaker em {
  background: url("/icons-svg/icon-speaker.svg") center center no-repeat;
}
.btn.icon-star em {
  background: url("/icons-svg/icon-star.svg") center center no-repeat;
}
.btn.icon-store em {
  background: url("/icons-svg/icon-store.svg") center center no-repeat;
}
.btn.icon-tablet em {
  background: url("/icons-svg/icon-tablet.svg") center center no-repeat;
}
.btn.icon-tag em {
  background: url("/icons-svg/icon-tag.svg") center center no-repeat;
}
.btn.icon-thumb-down em {
  background: url("/icons-svg/icon-thumb-down.svg") center center no-repeat;
}
.btn.icon-thumb-up em {
  background: url("/icons-svg/icon-thumb-up.svg") center center no-repeat;
}
.btn.icon-trash em {
  background: url("/icons-svg/icon-trash.svg") center center no-repeat;
}
.btn.icon-trending-down em {
  background: url("/icons-svg/icon-trending-down.svg") center center no-repeat;
}
.btn.icon-trending-up em {
  background: url("/icons-svg/icon-trending-up.svg") center center no-repeat;
}
.btn.icon-trophy em {
  background: url("/icons-svg/icon-trophy.svg") center center no-repeat;
}
.btn.icon-upload em {
  background: url("/icons-svg/icon-upload.svg") center center no-repeat;
}
.btn.icon-user em {
  background: url("/icons-svg/icon-user.svg") center center no-repeat;
}
.btn.icon-user-check em {
  background: url("/icons-svg/icon-user-check.svg") center center no-repeat;
}
.btn.icon-user-minus em {
  background: url("/icons-svg/icon-user-minus.svg") center center no-repeat;
}
.btn.icon-user-plus em {
  background: url("/icons-svg/icon-user-plus.svg") center center no-repeat;
}
.btn.icon-video em {
  background: url("/icons-svg/icon-video.svg") center center no-repeat;
}
.btn.icon-view em {
  background: url("/icons-svg/icon-view.svg") center center no-repeat;
}
.btn.icon-x em {
  background: url("/icons-svg/icon-x.svg") center center no-repeat;
}
.btn.icon-x-circle em {
  background: url("/icons-svg/icon-x-circle.svg") center center no-repeat;
}
.btn.icon-x-square em {
  background: url("/icons-svg/icon-x-square.svg") center center no-repeat;
}
.btn.icon-zoom-in em {
  background: url("/icons-svg/icon-zoom-in.svg") center center no-repeat;
}
.btn.icon-zoom-out em {
  background: url("/icons-svg/icon-zoom-out.svg") center center no-repeat;
}

</style>