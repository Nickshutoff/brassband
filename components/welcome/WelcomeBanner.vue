<template>
  <div class="banner">
    <h1 class="title">{{text.title}}</h1>
    <h1 class="subtitle">{{text.subtitle}}</h1>
  </div>
</template>

<script>
export default {
  name: 'BrassbandWelcomeBanner',

  data() {
    return {
      text: {
        title: 'MEGAPOLIS',
        subtitle: 'brass-band'
      }
    };
  },
};
</script>

<style lang="scss" scoped>
.banner {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-family: $font-title;
  font-size: 90px;
  letter-spacing: 2px;
  color: var(--c-400);
  transform: rotate(-4.28deg);
  user-select: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
}
.subtitle {
  font-size: 40px;
  margin-left: 365px;
  -webkit-text-stroke: var(--c-400) 1px;
  -webkit-text-fill-color: transparent;
}
</style>