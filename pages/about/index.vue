<template>
  <div class="flex flex-col min-h-screen overflow-hidden">
    <!-- Page content -->
    <main class="flex-grow">

      <!-- Page illustration -->
      <div class="relative max-w-6xl mx-auto h-0 pointer-events-none" aria-hidden="true">
        <PageIllustration />
      </div>

      <!-- Page sections -->
      <HeroAbout />
      <!-- <TeamImages /> -->
      <Timeline />
      <!-- <Team /> -->
      <!-- <TestimonialsCarousel /> -->
      <!-- <Career />
      <Clients /> -->
      <div class="max-w-6xl mx-auto px-4 sm:px-6 relative">
      <div class="pb-12 md:pb-20">
        <div class="max-w-3xl mx-auto text-center">
          <h1 class="h1 mb-4" data-aos="fade-up">Let's Chat! 👋</h1>
          <a class="h3 text-purple-600 hover:text-gray-200 transition duration-150 ease-in-out" href="#0">hi@akinhwan.com</a>
          <br>
          <a href="https://twitter.com/intent/user?screen_name=akinhwan" class="h3 text-purple-600 hover:text-gray-200 transition duration-150 ease-in-out twitter-mention-button" data-show-count="false">@Akinhwan</a>
          <!-- <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> -->
          <!-- <p class="text-xl text-gray-400 mb-8" data-aos="fade-up" data-aos-delay="200">
            Here is a timeline of my life and all the significant events thus far. 
            <br>And more excitingly, those to come!</p> -->
        </div>
      </div>
    </div>
      <Newsletter />
    </main>
  </div>
</template>

<script>
import Header from '~/partials/Header.vue'
import PageIllustration from '~/partials/PageIllustration.vue'
import HeroAbout from '~/partials/HeroAbout.vue'
import Timeline from '~/partials/Timeline.vue'
import Newsletter from '~/partials/Newsletter.vue'
import Footer from '~/partials/Footer.vue'

export default {
  name: 'About',
  components: {
    Header,
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