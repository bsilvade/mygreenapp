<template>
  <div id="home-page" class="page-wrapper home-page">
    <site-hero
      :title="title"
      :subtitle="subtitle"
      :image="featureImage"
      :showvideo="true"
    >
      <button
        v-if="$siteConfig.newsletter.on"
        class="button is-primary"
        @click="$eventBus.$emit('modal-triggered', 'newsletter-modal')"
      >
        Subscribe To Newsletter
      </button>
    </site-hero>
    <main-section theme="one-column">
      <template v-slot:default>
        <style>
          @media screen and (max-device-width: 480px) {
            .mobileSite {
              display: none;
            }
          }
        </style>
        <div style="margin:50px,text-align: center" class="mobileSite">
          <!-- p class="line-1 anim-typewriter title animated fadeInUp">
            More coming soon... Please stay tuned!
          </p -->
        </div>
        <!-- All Posts -->
        <posts-grid />
      </template>
      <template v-slot:sidebar>
        Nothing here
      </template>
    </main-section>
    <news-letter-form-modal />
  </div>
</template>

<script>
import { mapState } from 'vuex'
import { setPageData } from '../helper'
import NewsLetterFormModal from '~/components/NewsLetterFormModal'

export default {
  name: 'HomePage',
  head() {
    return {
      title: `Home | ${this.$siteConfig.siteName}`
    }
  },
  components: {
    NewsLetterFormModal
  },
  computed: {
    ...mapState(['title', 'subtitle', 'featureImage'])
  },
  fetch({ store, params }) {
    setPageData(store, { slug: 'home' })
  }
}
</script>

<style>
.home-page .under-subtitle {
  border-top: none;
}
.line-1 {
  position: relative;
  top: 50%;
  width: 24em;
  margin: 0 auto;
  border-right: 2px solid rgba(255, 255, 255, 0.75);
  font-size: 180%;
  font-family: monospace;
  text-align: center;
  white-space: nowrap;
  overflow: hidden;
  transform: translateY(-50%);
}
/* Animation */
.anim-typewriter {
  animation: typewriter 5s steps(30) 1s 1 normal both,
    blinkTextCursor 600ms steps(30) infinite normal;
}
@keyframes typewriter {
  from {
    width: 0;
  }
  to {
    width: 24em;
  }
}
@keyframes blinkTextCursor {
  from {
    border-right-color: black;
  }
  to {
    border-right-color: transparent;
  }
}
</style>
