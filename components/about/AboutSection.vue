<template>
  <div id="about" class="about">
    <HeadingComponent class="about-item flex1" :heading="text.heading" />
    <AboutText class="about-item flex2" />
    <ButtonTemplate class="about-item flex3" :text="text.button"/>
    <img class="about-item flex4" :src="img.src" :alt="img.alt">
  </div>
</template>

<script>
import HeadingComponent from '../common/HeadingComponent.vue';
import AboutText from './AboutText.vue';
import ButtonTemplate from '../common/ButtonTemplate.vue';

export default {
  name: 'BrassbandAbout',

  components: {
    HeadingComponent,
    AboutText,
    ButtonTemplate,
  },

  data() {
    return {
      text: {
        heading: 'КТО МЫ?',
        button: 'Узнать стоимость'
      },
      img: {
        src: require('~/assets/img/photos/1.png'),
        alt: 'Фото бэнда 1'
      }
    };
  },
};
</script>

<style lang="scss" scoped>
.about {
  padding;
  display: flex;
  align-items: center;
  &-item {
    display: flex;
  }
}

</style>