<template>
  <div class="container">
    <HeaderContainer />
  </div>
</template>

<script>
import HeaderContainer from '~/components/header/HeaderContainer.vue'

export default {
  name: 'IndexPage',
  components: {
    HeaderContainer,
  }
}
</script>

<style lang="scss">
.container {
  max-width: 1440px;
}
</style>