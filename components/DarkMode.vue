<template>
  <!-- <button type="button" class="inline-block rounded-full text-white leading-normal uppercase shadow-md hover:bg-blue-700 hover:shadow-lg focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0 active:bg-blue-800 active:shadow-lg transition duration-150 ease-in-out w-9 h-9">
      test
  </button> -->
  <div>
    <!-- <p class="p-4 pb-2">
      <select
        v-model="$colorMode.preference"
        class="
          w-24
          h-8
          dark:bg-gray-900 dark:text-white dark:border-gray-700
        "
        @change="check()"
      >
        <option value="system">System</option>
        <option value="light">Light</option>
        <option value="dark">Dark</option>
      </select>
    </p> -->
    <input
          v-model="$colorMode.preference"
          :class="($colorMode.value === 'dark')? 'toggle-1' : ''"
          :value="mode"
          class="toggle"
          type="checkbox"
          @change="check()" />
  </div>
</template>

<script>
export default {
  name: 'DarkMode',
  data () {
    return {
      mode: !(this.$colorMode.value === 'light') ? 'light' : 'dark'
    }
  },
  methods: {
    check (event) {
      console.log(this.$colorMode)
      this.$colorMode.preference = !(this.$colorMode.value === 'light') ? 'light' : 'dark'
    }
  }
}
</script>

<style>
.toggle {
  --size: 1.5rem;
  appearance: none;
  outline: none;
  cursor: pointer;
  width: var(--size);
  height: var(--size);
  box-shadow: inset calc(var(--size) * 0.33) calc(var(--size) * -0.25) 0;
  border-radius: 999px;
  color: #cacadc;
  transition: all 500ms;
}
.toggle-1 {
  --ray-size: calc(var(--size) * -0.4);
  --offset-orthogonal: calc(var(--size) * 0.65);
  --offset-diagonal: calc(var(--size) * 0.45);
  transform: scale(0.75);
  color: #fa0;
  box-shadow: inset 0 0 0 var(--size),
    calc(var(--offset-orthogonal) * -1) 0 0 var(--ray-size),
    var(--offset-orthogonal) 0 0 var(--ray-size),
    0 calc(var(--offset-orthogonal) * -1) 0 var(--ray-size),
    0 var(--offset-orthogonal) 0 var(--ray-size),
    calc(var(--offset-diagonal) * -1) calc(var(--offset-diagonal) * -1) 0
      var(--ray-size),
    var(--offset-diagonal) var(--offset-diagonal) 0 var(--ray-size),
    calc(var(--offset-diagonal) * -1) var(--offset-diagonal) 0 var(--ray-size),
    var(--offset-diagonal) calc(var(--offset-diagonal) * -1) 0 var(--ray-size);
}
</style>
