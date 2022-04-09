<template>
  <div>
    <NavBar2 class="fixed z-50 w-full" />
    <HeroSection />
    <AboutSection />
    <ServiceSection />
    <TeamSection />
    <ContactSection />
    <CallToAction />
    <FooterSection />
  </div>
</template>

<script>
import NavBar2 from './components/NavBar2.vue'
import HeroSection from './components/HeroSection.vue'
import AboutSection from './components/AboutSection.vue'
import TeamSection from './components/TeamSection.vue'
import ServiceSection from './components/ServiceSection.vue'
import ContactSection from './components/ContactSection.vue'
import CallToAction from './components/CallToAction.vue'
import FooterSection from './components/FooterSection.vue'

export default {
  name: 'App',
  components: {
    NavBar2,
    HeroSection,
    AboutSection,
    TeamSection,
    ServiceSection,
    ContactSection,
    CallToAction,
    FooterSection,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
