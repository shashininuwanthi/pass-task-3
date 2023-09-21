<template>
  <div class="home">
    <NavBar />
    <HeroSection id="hero" />
    <AboutSection id="about" />
    <PortfolioSection id="portfolio" />
    <ContactSection id="contact" />
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar.vue';
import HeroSection from '@/components/HeroSection.vue';
import AboutSection from '@/components/AboutSection.vue';
import PortfolioSection from '@/components/PortfolioSection.vue';
import ContactSection from '@/components/ContactSection.vue';

export default {
  name: 'HomeView',
  components: {
    NavBar,
    HeroSection,
    AboutSection,
    PortfolioSection,
    ContactSection
  }
}
</script>
