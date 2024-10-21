<template>
  <div>
    <HeaderSection />
    <WelcomeSection />
    <AboutSection />
  </div>
</template>

<script>
import HeaderSection from '~/components/header/HeaderSection.vue'
import WelcomeSection from '~/components/welcome/WelcomeSection.vue';
import AboutSection from '~/components/about/AboutSection.vue';

export default {
  name: 'IndexPage',
  components: {
    HeaderSection,
    WelcomeSection,
    AboutSection,
  }
}
</script>

<style lang="scss">
</style>