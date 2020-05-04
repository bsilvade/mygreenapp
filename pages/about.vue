<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="About Us"
      subtitle=""
      image="/uploads/home-hero.jpg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>How can I make my life more sustainable?</h3>
          <p>
           We live in a world facing climate change, pollution, destruction of natural ecosystems &amp; many of us want to do better, would like to achieve zero carbon footprint, but they don’t know how to do it. 
          </p>
          <p>
          Pedro Teixeira and Bruno Sousa are businessmen that travel a lot by plane, and, despite our strong environmental concerns, we found that it’s not easy to assess our individual Carbon footprint. Our objective is to make it easier to all customers, individuals and organizations, to monitor and offset their Carbon footprint.
          </p>
          <p>
          Our motivation is to contribute to a better world and at the same develop our own sustainable business, scalable, global, digital, and innovative. 
          </p>
          <p>
          My Green App – Go green was born in October 2019 in Portugal &amp; Singapore.
          </p>
          <h3>Founders</h3>
           <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <h3>
                Pedro Teixeira
              </h3>
              <p class="subtitle">
                CEO
              </p>
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
              <h3>
                Bruno Sousa
              </h3>
              <p class="subtitle">
                CTO
              </p>
              IT Manager & Technology Strategist
              </br>
              14+ years experience
              </br>
              Lived in Portugal and Switzerland
              </br>
              Engineering Degree in Computing Science; MBA
              </br>
              Team Leader at CERN
              <img src="/uploads/Bruno Sousa.png" />
            </article>
          </div>
        </div>
        </div>
        </template>

      <template v-slot:sidebar>
        <h3 class="subtitle is-4">
          Latest Posts
        </h3>
        <posts-grid :per-row="1" :number="2" />
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
