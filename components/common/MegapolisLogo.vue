<template>
  <img :src='logo.src' :alt='logo.alt'>
</template>

<script>
export default {
  name: 'BrassbandMegapolisLogo',

  data() {
    return {
      logo: {
        src: require('~/assets/img/icons/logo.svg'),
        alt: 'Megapolis Brass-Band'
      }
    };
  },
};
</script>