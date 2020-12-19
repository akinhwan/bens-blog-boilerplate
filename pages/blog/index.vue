<script>
import BlogPostList from '~/components/BlogPostList'

export default {
  components: {
    BlogPostList
  },
  async asyncData({ $content }) {
    const posts = await $content('blog').fetch()

    return {
      posts
    }
  }
}
</script>

<template>
  <div class="content">
    <BlogPostList :list="posts" />
  </div>
</template>

<style lang="scss">
@import '../../styles/_settings.scss';


</style>
