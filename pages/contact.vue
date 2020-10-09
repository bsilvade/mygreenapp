<template>
  <div id="contact-page" class="page-wrapper contact-page content-page">
    <site-hero
      title="Contact Us"
      subtitle="Ideas or toughts? Get in touch!"
      image="/uploads/mga-contact.jpeg"
    ></site-hero>
    <main-section theme="sidebar-right">
      <template v-slot:default>
        <div class="tile is-ancestor">
          <div class="tile is-parent">
            <article class="tile is-child box">
              <contact-form />
            </article>
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

<template v-slot:sidebar>
      <h3 class="subtitle is-4">
          Latest
        </h3>
        <!-- Latest Posts -->
        <posts-grid :per-row="1" :number="2" />
      </template>
<script>
import ContactForm from '~/components/ContactForm'
export default {
  head() {
    return {
      title: `Contact | ${this.$siteConfig.siteName}`
    }
  },
  components: { ContactForm }
}
</script>
