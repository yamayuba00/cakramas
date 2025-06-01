<template>
  <Header/>
  <HeroSection/>
  <AboutSection/>
  <CoreValue/>
  <MissionSection/>
  <SolutionSection/>
  <ContactSection/>
  <FooterSection/>

</template>

<script setup>
import { ref } from 'vue'
import Header from './components/Header.vue';
import HeroSection from './components/HeroSection.vue';
import AboutSection from './components/AboutSection.vue';
import CoreValue from './components/CoreValue.vue';
import MissionSection from './components/MissionSection.vue';
import SolutionSection from './components/SolutionSection.vue';
import ContactSection from './components/ContactSection.vue';
import FooterSection from './components/FooterSection.vue';


components: {
  Header,
  HeroSection,
  AboutSection,
  CoreValue,
  MissionSection,
  SolutionSection,
  ContactSection,
  FooterSection
}

</script>