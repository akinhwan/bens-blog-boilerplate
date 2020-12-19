<script>
import PageIllustration from '../partials/PageIllustration.vue'
import HeroHome from '../partials/HeroHome.vue'
import Tabs from '../partials/Tabs.vue'
import News from '../partials/News.vue'
import Newsletter from '../partials/Newsletter.vue'
import Testimonials from '../partials/Testimonials.vue'

export default {
  name: 'Home',
  components: {
    PageIllustration,
    HeroHome,
    Testimonials,
    Tabs,
    News,
    Newsletter
  }
}
</script>

<template>
  <div class="flex flex-col min-h-screen overflow-hidden">
    <main class="flex-grow">
      <div
        class="relative max-w-6xl mx-auto h-0 pointer-events-none"
        aria-hidden="true"
      >
        <PageIllustration />
      </div>
      <HeroHome />
      <Tabs />
      <Testimonials />
      <News />
      <Newsletter />
    </main>
  </div>
</template>

<style lang="scss" scoped>
@import '../styles/_settings.scss';

// .button {
//   display: inline-block;
//   @apply mt-3;
//   font-size: 1.2rem;
//   font-family: $ff-serif;
//   color: #fff;
//   background-color: $c-primary;
//   padding: 0.8rem 1.6rem;
//   border-radius: 4px;
//   transition: background-color 0.1s ease;
// }

// .title {
//   @apply block;
//   @apply mt-3;
//   color: $c-navy;
//   font-family: $ff-sans;
//   @apply font-semibold;
//   @apply text-5xl;
//   letter-spacing: 1px;
// }

// .subtitle {
//   font-weight: 300;
//   font-size: 1.6rem;
//   line-height: 1.3;
//   color: #57708a;
//   padding-bottom: 15px;
//   font-family: $ff-serif;
// }
</style>
