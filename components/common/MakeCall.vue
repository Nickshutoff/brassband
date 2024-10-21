<template>
  <div class="make-call">
    <img :src="phoneIcon.src" :alt="phoneIcon.alt">
    <a :href="`tel:${phoneNumber}`" class="phone-link">
      <slot></slot>
    </a>
  </div>
</template>

<script>
export default {
  name: 'BrassbandMakeCall',

  data() {
    return {
      phoneIcon: {
        src: require('~/assets/img/icons/phone2.svg'),
        alt: 'Позвоните нам'
      }
    };
  },

  props: {
    phoneNumber: {
      type: String,
      required: true
    }
  }
};
</script>
<style lang="scss" scoped>
.make-call {
  display: flex;
  align-items: center;
  
  img {
    width: 24px;
  }
}
</style>