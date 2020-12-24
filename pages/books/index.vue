<template>
  <div class="flex flex-col min-h-screen overflow-hidden">
    <!-- Page content -->
    <main class="flex-grow">

      <!-- Page illustration -->
      <div class="relative max-w-6xl mx-auto h-0 pointer-events-none" aria-hidden="true">
        <PageIllustration />
      </div>

      <!-- Page sections -->
      <BlogSingle />
      <Newsletter />

    </main>
  </div>
</template>

<script>
import PageIllustration from '~/partials/PageIllustration.vue'
import BlogSingle from '~/partials/BlogSingle.vue'
import Newsletter from '~/partials/Newsletter.vue'

export default {
  name: 'BlogPost',
  components: {
    PageIllustration,
    BlogSingle,
    Newsletter
  }
};
</script>

<style lang="">
  
</style>