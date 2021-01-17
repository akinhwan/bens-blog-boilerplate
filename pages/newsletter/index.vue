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

      <div id="archive" class="max-w-3xl mx-auto text-center mb-8">
        <h2 class="h2 mb-4" data-aos="fade-up">Archive<br> 
        <!-- <p  class="h4">
          (just me talking to myself for now)
          </p> -->
          </h2>
          <div class="grid grid-cols-3">
            <div></div>
          <ol type="1" class='text-left mx-auto list-decimal'>
            <li class="mb-4 text-gray-400">
              <a class="text-xl hover:underline " href="https://eomail6.com/preview?p=60273194-461b-11eb-a3d0-06b4694bee2a&pt=automation&t=1610806707&s=d2619d274e98c71a74109cf86f4dc40e662e7a28e1db23d55aa2dab0dd552879">This is how it all begins...
</a>
            </li>
            <li class="mb-4 text-gray-400">
              <a class="text-xl hover:underline " href="https://eomail6.com/preview?p=7a3aea83-461f-11eb-a3d0-06b4694bee2a&pt=campaign&t=1609729281&s=0f1f9876e2b6b058ed42b94dc9029e75a15f922417f464a1613bb7f60d7b657d">Just Start</a>
            </li>
            <li class="mb-4 text-gray-400">
              <a class="text-xl hover:underline " href="https://eomail6.com/preview?p=4472351f-4d06-11eb-a3d0-06b4694bee2a&pt=campaign&t=1610334153&s=ce53c492364c5e0fdf00331401191d0a7b7c49b68dc34f6ae29e3cde1fb5ee58">Keep Moving</a>
            </li>
          </ol>
            <div></div>
          </div>
      </div>




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