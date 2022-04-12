<template>
  <div class="min-h-screen">
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 sm:static my-auto">
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
          Skills
        </h1>
      </div>
      <div class="grid grid-cols-2 gap-2">
        <div v-for="item, i in skills" :key="i">
          <div>
            <div class="p-6 ">
              <h5 class="text-gray-900 text-xl font-medium mb-2 dark:text-white">
                {{ item.title }}
              </h5>
              <p class="text-gray-700 dark:text-white text-base mb-4" v-html="item.des">
              </p>
              <!-- <p class="text-gray-600 text-xs">Last updated 3 mins ago</p> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skill_nuxt',
  data () {
    return {
      skills: [
        {
          title: 'Back-end Development',
          des: '<b>PHP</b>: Laravel<br><b>NodeJs</b>: MeteorJs, Express'
        },
        {
          title: 'Front-end Development',
          des: 'HTML, CSS, Javascript❤<br>Codova, Progressive Web App(PWA)<br><b>VueJs</b>: NuxtJS, Vuex'
        },
        {
          title: 'Databases',
          des: 'MongoDB, PostgreSQL, MySQL'
        },
        {
          title: 'Others',
          des: 'RestAPIs, GraphQL, Axios'
        }
      ]
    }
  }
}
</script>
