<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Our Partners"
      subtitle=""
      image="/uploads/mga-partners.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
        <div class="tile is-ancestor">
          <div class="tile is-parent">

            <a href="https://climatelaunchpad.org/">
            <figure class=" ">
              <opti-image
                :src="require('~/assets/uploads/ClimateLaunchpad-No-Background.png').src"
                :srcset="
                  require('~/assets/uploads/ClimateLaunchpad-No-Background.png').srcSet
                " width="250" height="250" 
              />
            </a>
            
            <a href="https://uptec.up.pt/">
              <figure class=" ">
                <opti-image
                  :src="require('~/assets/uploads/UPTEC.png').src"
                  :srcset="
                    require('~/assets/uploads/UPTEC.png').srcSet
                  " width="250" height="250" 
                />
            </a>
          </div>
        </div>
        </div>
        </template>

      <template v-slot:sidebar>
      <!-- h3 class="subtitle is-4">
          The Journey
        </h3 -->
        <!-- Latest Posts -->
        <!-- posts-grid :per-row="1" :number="2" / -->
      </template>
    </main-section>
  </div>
</template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `About | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
