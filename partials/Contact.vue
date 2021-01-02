<template>
  <div class="flex flex-col min-h-screen overflow-hidden">
    <!-- Page content -->
    <main class="flex-grow">

      <section class="relative">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 relative">
          <div class="pt-12 pb-12 md:pb-20">

            <!-- Page header -->
            <div class="max-w-3xl mx-auto text-center pb-12 md:pb-16">
              <h1 class="h1 mb-4" data-aos="fade-up">Leave a comment</h1>
              <p class="text-xl text-gray-400" data-aos="fade-up" data-aos-delay="200">The following fields are required.</p>
            </div>

            <!-- Contact form -->
            <form class="max-w-xl mx-auto">
              <div class="flex flex-wrap -mx-3 mb-4">
                <div class="w-full px-3">
                  <label class="block text-gray-300 text-sm font-medium mb-1" for="email">Email <span class="text-red-600">*</span></label>
                  <input id="email" type="email" class="form-input w-full text-gray-300" placeholder="Enter your email address" required />
                </div>
              </div>
              <div class="flex flex-wrap -mx-3 mb-4">
                <div class="w-full px-3">
                  <label class="block text-gray-300 text-sm font-medium mb-1" for="comment">Comment<span class="text-red-600">*</span></label>
                  <textarea id="comment" rows="4" class="form-textarea w-full text-gray-300" placeholder="Write your comment"></textarea>
                </div>
              </div>
              <div class="flex flex-wrap -mx-3 mt-6">
                <div class="w-full px-3">
                  <button class="btn text-white bg-purple-600 hover:bg-purple-700 w-full">Post Comment</button>
                </div>
              </div>
            </form>

          </div>
        </div>
      </section>

      <Newsletter />

    </main>

  </div>
</template>

<script>
import Newsletter from './../partials/Newsletter.vue'

export default {
  name: 'Contact',
  components: {
    Newsletter
  },
};
</script>
