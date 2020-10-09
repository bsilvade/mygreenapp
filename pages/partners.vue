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
            <div id="left">
              <h3>
                Pedro Teixeira
              </h3>
              <p class="subtitle">
                CEO
              </p>
            </div>
              <div id="right" style="float:right">
               <figure class=" ">
                <opti-image
                  :src="require('~/assets/uploads/Pedro Teixeira.png').src"
                  :srcset="
                    require('~/assets/uploads/Pedro Teixeira.png').srcSet
                  " width="125" height="125" 
                />
              </div>
              <div>
              Regional Director in a listed MNC 
              </br>
              15+ years in P&L & M&S experience
              </br>
              Lived in Portugal, UK, Doha & Singapore
              </br>
              Master in Engineering; MBA
              </br>
              Top 10 in the Portuguese 40 Under 40 Award
            </article>
          </div>
          
          <div class="tile is-parent">
            <article class="tile is-child box">
              <div id="left">
              <h3>
                Bruno Sousa
              </h3>
              <p class="subtitle">
                CTO
              </p>
              </div>
              <div id="right" style="float:right">
               <figure class=" ">
                <opti-image
                  :src="require('~/assets/uploads/Bruno Sousa.png').src"
                  :srcset="
                    require('~/assets/uploads/Bruno Sousa.png').srcSet
                  " width="125" height="125" 
                />
              </div>
              <div>
              IT Manager & Technology Strategist
              </br>
              14+ years experience
              </br>
              Lived in Portugal and Switzerland
              </br>
              Engineering Degree in Computing Science; MBA
              </br>
              Team Leader at CERN
              </figure>
              </div>
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
