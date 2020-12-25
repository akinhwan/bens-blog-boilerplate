<script>
export default {
  async asyncData(ctx) {
    const page = await ctx.$content(`blog/${ctx.params.slug}`).fetch()
    return {
      page
    }
  },
  computed: {
  }
}
</script>

<template>
  <main>
    <article class="content">
      <p class="text-gray-500 blog-publish-date">{{ page.date }}</p>
      <h1 class="text-white blog-title">{{ page.title }}</h1>
      <nuxt-content class="text-white" :document="page" />
    </article>
  </main>
</template>

<style lang="scss">
@import '../../styles/_settings.scss';

.blog-publish-date {
  @apply mt-12;
}

.blog-title {
  @apply font-bold;
  @apply text-5xl;
  @apply mb-4;
}

.content {
  @apply mx-auto;
  @apply px-8;
  max-width: 740px;
}

.nuxt-content {
  * {
    color: #9ba9b4;
  }

  h2 {
    @apply font-bold;
    @apply mt-5 mb-5;
    @apply pb-3;
    border-bottom: 1px solid $c-border;
    @apply text-4xl;
    font-size: 2rem;
    line-height: 1.3;
  }

  h3 {
    @apply font-bold;
    @apply mt-5;
    @apply pb-3;
    font-size: 1.5rem;
    line-height: 1.3;
  }

  p,
  li {
    line-height: 1.7;
    font-size: 16px;

    @include breakpoint(600px) {
      font-size: 18px;
    }
  }

  li > ul > li {
        padding-left: 2rem;

  }

  p {
    @apply mb-4;
  }

  ul,
  ol {
    @apply list-decimal;
    @apply list-inside;
    @apply mb-4;
  }
}
</style>
