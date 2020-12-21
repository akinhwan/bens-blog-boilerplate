<script type="module">
import AppFooter from '~/components/AppFooter'
import AppNavbar from '~/components/AppNavbar'
// import AOS from 'aos'
// import { focusHandling } from 'cruip-js-toolkit'

export default {
  name: 'App',
  components: {
    AppFooter,
    AppNavbar
  },
  // mounted() {
  //   AOS.init({
  //     once: true,
  //     disable: 'phone',
  //     duration: 600,
  //     easing: 'ease-out-sine',
  //   })
  //   focusHandling()
  //   // Route change
  //   if (this.$router) {
  //     this.$watch('$route', () => {
  //       focusHandling()
  //     });
  //   }    
  // }  
}
</script>

<template>
  <div class="flex flex-col min-h-screen">
    <AppNavbar />
    <nuxt class="flex-1" />
    <AppFooter />
  </div>
</template>

<style>
/* @import '../styles/style.scss'; */

html {
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  background-color: #151719;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.content {
  @apply mx-auto;
  @apply px-8;
  max-width: 740px;
}
</style>
