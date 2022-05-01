<template>
  <div class="dark:bg-black dark:text-white bg-gray-100">
    <Nav @gotoElement="gotoElement"/>
    <div ref="home" class="overflow-hidden">
      <Home />
    </div>
    <div ref="about" style="transition: 1.5s all cubic-bezier(0.39, 0.575, 0.565, 1);">
      <About />
    </div>
    <div ref="career">
      <Career />
    </div>
    <div ref="skills">
      <Skill />
    </div>
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  methods: {
    gotoElement (link) {
      const element = this.$refs[link]
      if (!element) { return }
      window.scrollTo({ top: element.offsetTop, behavior: 'smooth' })
    }
  }
}
</script>

<style>
  .blob {
    position: absolute;
    top: 0;
    left: 0;
    fill: #023F92;
    width: 50vmax;
    z-index: 0;
    animation: move 10s ease-in-out infinite;
    transform-origin: 50% 50%;
  }

  @keyframes move {
    0%   { transform: scale(1)   translate(10px, -30px); }
    38%  { transform: scale(0.8, 1) translate(80vw, 30vh) rotate(160deg); }
    40%  { transform: scale(0.8, 1) translate(80vw, 30vh) rotate(160deg); }
    78%  { transform: scale(1.3) translate(0vw, 50vh) rotate(-20deg); }
    80%  { transform: scale(1.3) translate(0vw, 50vh) rotate(-20deg); }
    100% { transform: scale(1)   translate(10px, -30px); }
  }
</style>
