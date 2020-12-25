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

      <FeaturesBlocks />


      <!-- Simple Newsletter box -->
      <div class="max-w-6xl mx-auto px-4 sm:px-6 pb-10">
        <!-- CTA box -->
        <div class="relative py-10 px-8 md:py-16 md:px-12" data-aos="fade-up">
          <div class="relative flex flex-col lg:flex-row justify-between items-center">
            <!-- CTA form -->
            <form class="m-auto w-full lg:w-1/2 embeddable-buttondown-form"
              action="https://buttondown.email/api/emails/embed-subscribe/akinhwan" method="post" target="popupwindow"
              onsubmit="window.open('https://buttondown.email/akinhwan', 'popupwindow')">
              <div class="flex flex-col sm:flex-row justify-center max-w-xs mx-auto sm:max-w-md lg:max-w-none">
                <input type="email"
                  class="w-full appearance-none  border border-purple-500 focus:border-purple-300 rounded-sm px-4 py-3 mb-2 sm:mb-0 sm:mr-2 text-white placeholder-purple-400"
                  placeholder="Email Address…" aria-label="Email Address…" name="email" id="bd-email" />
                <input type="hidden" value="1" name="embed" />
                <!-- <a class="btn text-purple-600 bg-purple-100 hover:bg-white shadow" href="#0">Subscribe</a> -->
                <input type="submit" value="Subscribe"
                  class="btn text-white bg-purple-700 hover:bg-purple-600 shadow" />
              </div>
              <!-- Success message -->
              <!-- <p class="text-center lg:text-left lg:absolute mt-2 opacity-75 text-sm">Thanks for subscribing!</p> -->
            </form>

          </div>

        </div>

      </div>

      <Stats />

      <div class="max-w-3xl mx-auto text-center">
        <h2 class="h2 mb-4" data-aos="fade-up">Testimonials coming very soon! <br> <p  class="h4">
          (just me talking to myself for now)
          </p>
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
  import Newsletter from '~/partials/Newsletter.vue'
  import FeaturesBlocks from '~/partials/FeaturesBlocks.vue'

  export default {
    name: 'NewsletterPage',
    components: {
      Stats,
      FeaturesBlocks,
      TestimonialsCarousel,
      Newsletter
    },
  };
</script>

<style lang="">
  
</style>