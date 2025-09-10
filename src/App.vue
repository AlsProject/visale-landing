<template>
  <div id="app">
    <Header />
    <Hero />
    <WhyChooseUs />
    <WhoCanApply />
    <WorkFlow />
    <ClientsTrust />
    <Footer />
  </div>
</template>

<script>
import Header from './components/landingPage/Header.vue'
import Hero from './components/landingPage/Hero.vue'
import WhyChooseUs from './components/landingPage/WhyChooseUs.vue'
import WhoCanApply from './components/landingPage/WhoCanApply.vue'
import WorkFlow from './components/landingPage/WorkFlow.vue'
import ClientsTrust from './components/landingPage/ClientsTrust.vue'
import Footer from './components/landingPage/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    WhyChooseUs,
    WhoCanApply,
    WorkFlow,
    ClientsTrust,
    Footer
  }
}
</script>

<style>
#app {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
</style>
