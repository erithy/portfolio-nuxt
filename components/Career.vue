<template>
  <div class="min-h-screen">
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 sm:static">
      <div class="sm:max-w-lg">
        <h1
          class="
            pb-10
            text-4xl
            font font-extrabold
            tracking-tight
            dark:text-blue-500
            text-gray-900
            sm:text-6xl
          "
        >
          Resume
        </h1>
      </div>
      <div v-for="i in 5" :key="i">
      <div class="flex justify-center">
        <div
          class="
            flex flex-col
            md:flex-row md:max-w-xl
            rounded-lg
            dark:bg-black
            bg-white
            shadow-lg
            m-5
          "
        >
          <div class="p-6 flex flex-col justify-start">
            <h5 class="text-gray-900 text-xl font-medium mb-2 dark:text-white">
              Card title
            </h5>
            <p class="text-gray-700 dark:text-white text-base mb-4">
              This is a wider card with supporting text below as a natural
              lead-in to additional content. This content is a little bit
              longer.
            </p>
            <p class="text-gray-600 text-xs">Last updated 3 mins ago</p>
          </div>
        </div>
      </div>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Career_nuxt',
  data () {
    return {
      careers: [
        {
          year: '',
          des: ''
        }
      ]
    }
  }
}
</script>

<style>
  /* Styles required only for the example above */
  .scrollspy-example {
    position: relative;
    height: 200px;
    overflow: auto;
  }
</style>
