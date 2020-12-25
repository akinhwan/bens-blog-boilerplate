<template>
  <section class="relative">
    <div class="max-w-6xl mx-auto px-4 sm:px-6">
      <div class="pb-12 md:pt-40 md:pb-20">

        <!-- Page header -->
        <div class="max-w-3xl pb-12 md:pb-20 text-center md:text-left">
          <h1 class="h1" data-aos="fade-up">Read my writings on life, lessons, and the pursuit of happiness.</h1>
        </div>

        <!-- Featured article -->
        <div class="pb-12 md:pb-20">
          <article
            class="max-w-sm mx-auto md:max-w-none grid md:grid-cols-2 gap-6 md:gap-8 lg:gap-12 xl:gap-16 items-center">
            <router-link to="/blog-post" class="relative block group" data-aos="fade-right" data-aos-delay="200">
              <div
                class="absolute inset-0 bg-gray-800 hidden md:block transform md:translate-y-2 md:translate-x-4 xl:translate-y-4 xl:translate-x-8 group-hover:translate-x-0 group-hover:translate-y-0 transition duration-700 ease-out pointer-events-none"
                aria-hidden="true"></div>
              <figure
                class="relative h-0 pb-9/16 md:pb-3/4 lg:pb-9/16 overflow-hidden transform md:-translate-y-2 xl:-translate-y-4 group-hover:translate-x-0 group-hover:translate-y-0 transition duration-700 ease-out">
                <img
                  class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                  :src="require('~/assets/tc-crop-purple.png')" width="540" height="303" alt="Blog post 01">
              </figure>
            </router-link>
            <div data-aos="fade-left" data-aos-delay="200">
              <header>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out"
                        href="#0">Product</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out"
                        href="#0">Engineering</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h3 text-2xl lg:text-3xl mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">My 2020
                    Annual Review.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Habits I added and removed. Lessons I learned. Failures I made.
                In all realms Relationships, Financial, Health, Work, and Play. </p>
              <footer class="flex items-center mt-4">
                <!-- <a href="#0">
                  <img class="rounded-full flex-shrink-0 mr-4" :src="require('~/assets/news-author-04.jpg')" width="40" height="40" alt="Author 04">
                </a> -->
                <div>
                  <!-- <a class="font-medium text-gray-200 hover:text-gray-100 transition duration-150 ease-in-out" href="#0">Chris Solerieu</a>
                  <span class="text-gray-700"> - </span> -->
                  <span class="text-gray-500">Jan 1, 2021</span>
                </div>
              </footer>
            </div>
          </article>
        </div>

        <!-- Articles list -->
        <div class="max-w-sm mx-auto md:max-w-none">

          <!-- Section title -->
          <h4 class="h4 pb-6 mb-10 border-b border-gray-700" data-aos="fade-up">Latest articles</h4>

          <!-- Articles container -->
          <div class="grid gap-12 md:grid-cols-3 md:col-gap-6 md:row-gap-8 items-start">

            <!-- 1st article -->
            <article class="flex flex-col h-full" data-aos="fade-up">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      :src="require('~/assets/books.jpg')" width="352" height="198" alt="News 01" />
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out"
                        href="#0">Product</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out"
                        href="#0">Engineering</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">
                    Publishing here very soon!</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <!-- <a href="#0">
                  <img class="rounded-full flex-shrink-0 mr-4" :src="require('~/assets/news-author-01.jpg')" width="40" height="40" alt="Author 01" />
                </a> -->
                <div class="font-medium">
                  <!-- <a class="text-gray-200 hover:text-gray-100 transition duration-150 ease-in-out" href="#0">Anastasia Dan</a> -->
                  <!-- <span class="text-gray-700"> - </span> -->
                  <span class="text-gray-500">Jan 17, 2020</span>
                </div>
              </footer>
            </article>

            <!-- 2nd article -->
            <article class="flex flex-col h-full" data-aos="fade-up" data-aos-delay="200">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      :src="require('~/assets/podcast.jpg')" width="352" height="198" alt="News 02" />
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-pink-500 hover:bg-pink-600 transition duration-150 ease-in-out"
                        href="#0">Desing</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out"
                        href="#0">Engineering</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">
                    Publishing here very soon!</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <!-- <a href="#0">
                  <img class="rounded-full flex-shrink-0 mr-4" :src="require('~/assets/news-author-02.jpg')" width="40" height="40" alt="Author 02" />
                </a> -->
                <div class="font-medium">
                  <!-- <a class="text-gray-200 hover:text-gray-100 transition duration-150 ease-in-out" href="#0">Markus Barker</a>
                  <span class="text-gray-700"> - </span> -->
                  <span class="text-gray-500">Jan 12, 2020</span>
                </div>
              </footer>
            </article>

            <!-- 3rd article -->
            <article class="flex flex-col h-full" data-aos="fade-up" data-aos-delay="400">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img
                      class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out"
                      :src="require('~/assets/music.jpg')" width="352" height="198" alt="News 03" />
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out"
                        href="#0">Product</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-teal-500 hover:bg-teal-600 transition duration-150 ease-in-out"
                        href="#0">Tutorials and articles</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">
                    Publishing here very soon!</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">

                  <span class="text-gray-500">Jan 9, 2020</span>
                </div>
              </footer>
            </article>

            <!-- 4th article -->
            <!-- <article class="flex flex-col h-full" data-aos="fade-up">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out" :src="require('~/assets/news-04.jpg')" width="352" height="198" alt="News 04">
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out" href="#0">Product</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-green-500 hover:bg-green-600 transition duration-150 ease-in-out" href="#0">Culture</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">Publishing new articles soon, you're early to the party!.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">
                  <span class="text-gray-500">Jan 7, 2021</span>
                </div>
              </footer>
            </article> -->

            <!-- 5th article -->
            <!-- <article class="flex flex-col h-full" data-aos="fade-up" data-aos-delay="100">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out" :src="require('~/assets/news-05.jpg')" width="352" height="198" alt="News 05">
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out" href="#0">Engineering</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">Publishing new articles soon, you're early to the party!.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">
                  
                  <span class="text-gray-500">Jan 4, 2021</span>
                </div>
              </footer>
            </article> -->

            <!-- 6th article -->
            <!-- <article class="flex flex-col h-full" data-aos="fade-up" data-aos-delay="200">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out" :src="require('~/assets/news-06.jpg')" width="352" height="198" alt="News 06">
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-pink-500 hover:bg-pink-600 transition duration-150 ease-in-out" href="#0">Desing</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-teal-500 hover:bg-teal-600 transition duration-150 ease-in-out" href="#0">Tutorials and articles</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">Publishing new articles soon, you're early to the party!.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">
                  <span class="text-gray-500">Jan 2, 2021</span>
                </div>
              </footer>
            </article> -->

            <!-- 7th article -->
            <!-- <article class="flex flex-col h-full" data-aos="fade-up">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out" :src="require('~/assets/news-07.jpg')" width="352" height="198" alt="News 07">
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out" href="#0">Product</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out" href="#0">Engineering</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">Publishing new articles soon, you're early to the party!.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">
                  <span class="text-gray-500">Dec 24, 2019</span>
                </div>
              </footer>
            </article> -->

            <!-- 8th article -->
            <!-- <article class="flex flex-col h-full" data-aos="fade-up" data-aos-delay="100">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out" :src="require('~/assets/news-08.jpg')" width="352" height="198" alt="News 08">
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-blue-500 hover:bg-blue-600 transition duration-150 ease-in-out" href="#0">Engineering</a>
                    </li>
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-green-500 hover:bg-green-600 transition duration-150 ease-in-out" href="#0">Culture</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">Publishing new articles soon, you're early to the party!.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">
                  <span class="text-gray-500">Dec 12, 2019</span>
                </div>
              </footer>
            </article> -->

            <!-- 9th article -->
            <!-- <article class="flex flex-col h-full" data-aos="fade-up" data-aos-delay="200">
              <header>
                <router-link to="/blog-post" class="block mb-6">
                  <figure class="relative h-0 pb-9/16 overflow-hidden rounded-sm">
                    <img class="absolute inset-0 w-full h-full object-cover transform hover:scale-105 transition duration-700 ease-out" :src="require('~/assets/news-09.jpg')" width="352" height="198" alt="News 09">
                  </figure>
                </router-link>
                <div class="mb-3">
                  <ul class="flex flex-wrap text-xs font-medium -m-1">
                    <li class="m-1">
                      <a class="inline-flex text-center text-gray-100 py-1 px-3 rounded-full bg-purple-600 hover:bg-purple-700 transition duration-150 ease-in-out" href="#0">Product</a>
                    </li>
                  </ul>
                </div>
                <h3 class="h4 mb-2">
                  <router-link to="/blog-post" class="hover:text-gray-100 transition duration-150 ease-in-out">Publishing new articles soon, you're early to the party!.</router-link>
                </h3>
              </header>
              <p class="text-lg text-gray-400 flex-grow">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
              <footer class="flex items-center mt-4">
                <div class="font-medium">
                  <span class="text-gray-500">Dec 7, 2019</span>
                </div>
              </footer>
            </article> -->
          </div>

        </div>

        <!-- Pagination -->
        <nav class="flex justify-center pt-16" role="navigation" aria-label="Pagination Navigation">
          <ul class="inline-flex flex-wrap font-medium text-sm -m-1">
            <li class="m-1">
              <span
                class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-4 rounded-full text-gray-500">Prev</span>
            </li>
            <li class="m-1">
              <a href="#0"
                class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-2 rounded-full text-gray-300 hover:bg-purple-600 transition-colors duration-150 ease-in-out">1</a>
            </li>
            <!-- <li class="m-1">
              <a href="#0" class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-2 rounded-full text-gray-300 hover:bg-purple-600 transition-colors duration-150 ease-in-out">2</a>
            </li>
            <li class="m-1">
              <a href="#0" class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-2 rounded-full text-gray-300 hover:bg-purple-600 transition-colors duration-150 ease-in-out">3</a>
            </li>
            <li class="m-1">
              <span class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-2 rounded-full text-gray-500">...</span>
            </li> -->
            <!-- <li class="m-1">
              <a href="#0" class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-2 rounded-full text-gray-300 hover:bg-purple-600 transition-colors duration-150 ease-in-out">12</a>
            </li> -->
            <li class="m-1">
              <a href="#0"
                class="inline-flex h-10 min-w-10 justify-center items-center bg-gray-800 px-4 rounded-full text-gray-300 hover:bg-purple-600 transition-colors duration-150 ease-in-out">Next</a>
            </li>
          </ul>
        </nav>

      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: 'BlogList'
  }
</script>

<style lang="">
  
</style>