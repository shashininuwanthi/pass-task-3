<template>
  <div class="hero-container">
    <div class="hero-text-container">
        <p class = "hero-main-text head-text">HI! I AM SHASHINI</p>
        <p class = "hero-sub-text">Web Designer &</p>
        <p class = "hero-sub-text">Front End Developer</p>
    </div>
    <div class="hero-svg-container">
      <HeroSvg :width="'45vw'" :height="'45vw'" />
    </div>
  </div>
</template>
    <script>
import HeroSvg from "./svg/HeroSvg.vue";


export default {
  name: "HeroSection",
  components: {
    HeroSvg,
  },
};
</script>

    