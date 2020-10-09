<template>
  <div id="about-page" class="page-wrapper about-page content-page">
    <site-hero
      title="Vision"
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
        </div>
    </div>
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
