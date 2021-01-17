
<template>
  <div class="flex flex-col min-h-screen">
    <AppNavbar />
    <nuxt class="flex-1" />
    <AppFooter />
  </div>
</template>

<script>
import AppFooter from '~/components/AppFooter'
import AppNavbar from '~/components/AppNavbar'
// import { focusHandling } from 'cruip-js-toolkit'

export default {
  name: 'App',
  components: {
    AppFooter,
    AppNavbar
  },
  // mounted() {
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

<style lang="scss">
@import '../styles/_settings.scss';
@import '../assets/css/tailwind.css';


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
