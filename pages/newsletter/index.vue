<template>
  <div class="flex flex-col min-h-screen overflow-hidden">

    <section class="relative">
      <!-- Hero content -->
      <div class="max-w-6xl mx-auto px-4 mb-6 sm:px-6 relative">
        <div class="md:pt-40">
          <div class="max-w-3xl mx-auto text-center">
            <h1 class="h1 mb-4" data-aos="fade-up">I'm going Full-Time Maker</h1>
            <p class="text-xl text-gray-400 mb-8" data-aos="fade-up" data-aos-delay="200">
              Every <b>Sunday 10pm</b> EST in your Inbox, I'll share my process & progress.
              <br>
              The ups, the downs, and everything in between.
            </p>
          </div>
        </div>
      </div>
      <NewsletterSimple />
      <FeaturesBlocks />

      <Stats />

      <div class="max-w-3xl mx-auto text-center">
        <h2 class="h2 mb-4" data-aos="fade-up">Testimonials<br> 
        <!-- <p  class="h4">
          (just me talking to myself for now)
          </p> -->
          </h2>
      </div>
      <TestimonialsCarousel />

      <div class="max-w-6xl mx-auto px-4 mb-6 sm:px-6 relative">
        <div class="pt-24 pb-12 md:pb-20">
          <div class="max-w-3xl mx-auto text-center">
            <h1 class="h3 mb-4" data-aos="fade-up"> My Pledge to Readers</h1>
            <p class="text-xl text-gray-400 mb-8" data-aos="fade-up" data-aos-delay="200">
              I won't sell your email address to any third parties, and I won't use it for anything other than sending
              you
              an email once a week. Period.
            </p>
          </div>
        </div>
      </div>
      <Newsletter />
    </section>
  </div>
</template>


<script>
  import TestimonialsCarousel from '~/partials/TestimonialsCarousel.vue'
  import Stats from '~/partials/Stats.vue'
  import NewsletterSimple from '~/partials/NewsletterSimple.vue'
  import Newsletter from '~/partials/Newsletter.vue'
  import FeaturesBlocks from '~/partials/FeaturesBlocks.vue'

  export default {
    name: 'NewsletterPage',
    components: {
      Stats,
      FeaturesBlocks,
      TestimonialsCarousel,
      Newsletter,
      NewsletterSimple
    },
  };
</script>

<style lang="">
  
</style>