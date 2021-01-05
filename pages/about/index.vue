<template>
  <div class="flex flex-col min-h-screen overflow-hidden">
    <!-- Page content -->
    <main class="flex-grow">

      <div class="relative max-w-6xl mx-auto h-0 pointer-events-none" aria-hidden="true">
        <PageIllustration />
      </div>

      <HeroAbout />
      <Timeline />
      <div class="max-w-6xl mx-auto px-4 sm:px-6 relative">
      <div class="pb-12 md:pb-20">
        <div class="max-w-3xl mx-auto text-center">
          <h1 class="h1 mb-4" data-aos="fade-up">Let's Chat! 👋</h1>
          <a class="h3 text-purple-600 hover:text-gray-200 transition duration-150 ease-in-out" href="mailto:hi@akinhwan.com">hi@akinhwan.com</a>
          <br>
          <a href="https://twitter.com/intent/user?screen_name=akinhwan" class="h3 text-purple-600 hover:text-gray-200 transition duration-150 ease-in-out twitter-mention-button" data-show-count="false">@Akinhwan</a>
          <!-- <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> -->
          
        </div>
      </div>
    </div>
      <Newsletter />
    </main>
  </div>
</template>

<script>
import PageIllustration from '~/partials/PageIllustration.vue'
import HeroAbout from '~/partials/HeroAbout.vue'
import Timeline from '~/partials/Timeline.vue'
import Newsletter from '~/partials/Newsletter.vue'
import Footer from '~/partials/Footer.vue'

export default {
  name: 'About',
  components: {
    PageIllustration,
    HeroAbout,
    Timeline,
    Newsletter,
    Footer,
  },
};
</script>

<style lang="">
  
</style>