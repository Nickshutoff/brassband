<template>
  <div class="header-container">
    <MegapolisLogo />
    <nav class="header-navigation">
      <Navigation />
      <MakeCall phoneNumber="+79370923080">+7 937 092-30-80</MakeCall>
      <SocialNets />
    </nav>
  </div>
</template>

<script>
import MegapolisLogo from '~/components/common/MegapolisLogo.vue';
import MakeCall from '~/components/common/MakeCall.vue';
import SocialNets from '~/components/common/SocialNets.vue';
import Navigation from '~/components/header/Navigation.vue';


export default {
  name: 'BrassbandHeader',

  components: {
    MegapolisLogo,
    MakeCall,
    SocialNets,
    Navigation
  },
}
</script>

<style lang="scss" scoped>
  .header-container {
    display: flex;
    flex: 1;
    justify-content: center;
    margin: 51px 70px;
    gap: 20px;
    font-family: $font-primary;
  }

  .header-navigation {
    display: flex;
    flex-direction: row;
    gap: 105px;
    ::v-deep * {
      color: var(--c-600);
    }
  }
</style>