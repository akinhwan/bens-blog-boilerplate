<script>
export default {
  name: 'BlogPostPreview',
  props: {
    post: {
      type: Object,
      required: true
    }
  },
  computed: {
    // formatPublishDate() {
    //   const dateFormat = new Date(this.post.published)
    //   // const options = {
    //   //   year: 'numeric',
    //   //   month: 'long',
    //   //   day: 'numeric'
    //   // }
    //   console.log(dateFormat.toLocaleDateString('en-US'))

    //   return dateFormat.toLocaleDateString('en-US')
    // }
  }
}
</script>

<template>
    <nuxt-link class="" :to="post.path">
  <section class="blog-post mb-16">
    <time class="text-gray-500 blog-post__time">{{ post.date }}</time>
    <h2 class="h2 text-white blog-post__title">
      <a :href="post.path" class="blog-post__link">{{ post.title }}</a>
    </h2>
    <p v-if="post.excerpt" class="text-gray-300 blog-post__excerpt">{{ post.excerpt }}</p>
      <!-- Read More > -->
  </section>
    </nuxt-link>
</template>

<style lang="scss" scoped>
@import '../styles/_settings.scss';
// $primary-color: #22aaff;
$purple-400: #A78BFA;

.blog-post {
  // margin-bottom: 2.5rem;
}

.blog-post__button {
  display: inline-block;
}

.blog-post__excerpt {
  margin-top: 0;
  @apply mb-3;
  font-size: 1.2rem;
}

.blog-post__link {
  font-weight: 700;
  // color: #2c3e50;

  &:hover {
    text-decoration: underline;
  }
}

.blog-post__time {
  // font-family: 'Poppins';
  font-weight: 500;
}

.blog-post__title {
  margin-top: 0.5rem;
  margin-bottom: 0.75rem;
  @apply font-bold;
  // font-family: $ff-sans;
  @apply text-2xl;
}

.button {
  // font-family: 'Poppins';
  font-weight: 500;
  border: 1px solid $purple-400;
  border-radius: 4px;
  // color: $c-primary;
  font-size: 0.9rem;
  padding: 0.3rem 0.6rem;
  text-transform: uppercase;
  box-shadow: 0 0;
  transition: background-color 0.2s ease-in, color 0.2s ease-in;
}

.button:hover {
  color: #fff;
  text-decoration: none;
  background-color: $c-primary;
}

.tag-list {
  list-style: none;
  padding-left: 0;
  display: flex;
  margin-bottom: 25px;
}

.tag-list__item {
  margin-left: 10px;
}

.tag-list__item:first-child {
  margin-left: 0;
}

.tag-list__btn {
  padding: 5px;
  font-size: 0.9rem;
  background-color: #fff;
}
</style>
