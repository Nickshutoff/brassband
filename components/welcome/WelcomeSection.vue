<template>
  <div class="welcome-container">
    <WelcomeBanner />
    <p class="welcome-slogan">{{text.slogan}}</p>
    <!-- CAROUSEL HERE UNDER CONSTRUCTION -->
    <WelcomeMarquee />
  </div>
</template>

<script>
import WelcomeBanner from './WelcomeBanner.vue';
import WelcomeMarquee from './WelcomeMarquee.vue';

export default {
  name: 'BrassbandWelcome',
  components: {
    WelcomeBanner,
    WelcomeMarquee,
  },
  data() {
    return {
      text: {
        slogan: 'Наша главная цель — сделать ваш праздник ещё лучше.'
      }
    };
  },
}
</script>
<style lang="scss" scoped>
.welcome-container {
  display: flex;
  align-items: center;
  flex-direction: column;
}
.welcome-slogan {
  margin-top: 65px;
  font-family: $font-subtitle;
  font-size: 24px;
  color: var(--c-600);
}
</style>