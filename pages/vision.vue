<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Our Vision"
      subtitle=""
      image="/uploads/mga-vision.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="content">
          <h3>Our goal: achieve zero carbon footprint together</h3>
          <p>
          The world today is faced with climate change, pollution and destruction of natural ecosystems. One way to fight these threats to our planet and society is to achieve zero carbon footprint – balancing out man-made carbon dioxide emissions through reduction measures. 
          </p>
          <p>
          As two frequently travelling businessmen concerned with the increasing environmental problems, we realised that calculating our personal carbon footprint is a particularly hard task without a proper tool to help us. This is how My Green App was born.
          </p>
          <p>
          Our aim is to help people and organisations reduce their impact on nature by providing them with an easy and accessible tool to monitor and offset their carbon footprint. A step towards a more sustainable life.
          </p>
          <p>
          My Green App – Go green was born in October 2019 in Portugal &amp; Singapore.
          </p>
        </div>
    </div>
</template>

<template v-slot:sidebar>
      <class="subtitle is-4">
          Latest News
        </h3 -->
        <!-- Latest Posts -->
        <posts-grid :per-row="1" :number="2" />
      </template>
<script>
import QuoteCard from '~/components/cards/QuoteCard'
export default {
  head() {
    return {
      title: `Vision | ${this.$siteConfig.siteName}`
    }
  },
  components: { QuoteCard }
}
</script>
