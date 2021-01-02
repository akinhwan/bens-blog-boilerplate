<script>
export default {
  async asyncData(ctx) {
    const page = await ctx.$content(`blog/${ctx.params.slug}`).fetch()
    return {
      page
    }
  },
  head() {
      return {
        script: [
          {
            src:
              'https://unpkg.com/commentbox.io/dist/commentBox.min.js'
          }
        ],
        // link: [
        //   {
        //     rel: 'stylesheet',
        //     href: 'https://fonts.googleapis.com/css?family=Roboto&display=swap'
        //   }
        // ]
      }
    },
    mounted() {
    //   commentBox('5633211778465792-proj');
    //   commentBox('my-project-id', {
    //     backgroundColor: '#000',
    //     textColor: '#fff',
    //     className: 'commentbox', // the class of divs to look for
    //     defaultBoxId: 'commentbox', // the default ID to associate to the div
    //     tlcParam: 'tlc', // used for identifying links to comments on your page
    //     backgroundColor: null, // default transparent
    //     textColor: null, // default black
    //     subtextColor: null, // default grey
    //     singleSignOn: null, // enables Single Sign-On (for Professional plans only)
    //     /**
    //      * Creates a unique URL to each box on your page.
    //      * 
    //      * @param {string} boxId
    //      * @param {Location} pageLocation - a copy of the current window.location
    //      * @returns {string}
    //      */
    //     createBoxUrl(boxId, pageLocation) {

    //         pageLocation.search = ''; // removes query string!
    //         pageLocation.hash = boxId; // creates link to this specific Comment Box on your page
    //         return pageLocation.href; // return url string
    //     },
    //     /**
    //      * Fires once the plugin loads its comments.
    //      * May fire multiple times in its lifetime.
    //      * 
    //      * @param {number} count
    //      */
    //     onCommentCount(count) {

    //     }
    // });
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
    <!-- <div class="commentbox"></div> -->
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

  a {
    color: #5d5dff;
    // text-decoration: underline;
  }

  a:hover {
    text-decoration: underline;
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
