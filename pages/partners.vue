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
            <article class="tile is-child box">
               <figure class=" ">
                <opti-image
                  :src="require('~/assets/uploads/ClimateLaunchpad-No-Background.png').src"
                  :srcset="
                    require('~/assets/uploads/ClimateLaunchpad-No-Background.png').srcSet
                  " width="175" height="175" 
                />
            </article>
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
