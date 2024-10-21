<template>
  <div class="marquee-container">
    <div class="marquee">
      <span>{{ text.first }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.second }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.third }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.first }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.second }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.third }}</span>
      <img :src="carrier.src" :alt="carrier.alt">

      <span>{{ text.first }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.second }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.third }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.first }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.second }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
      <span>{{ text.third }}</span>
      <img :src="carrier.src" :alt="carrier.alt">
    </div>
  </div>
</template>

<script>
export default {
  name: 'BrassbandWelcomeMarquee',

  data() {
    return {
      text: {
        first: 'Выступаем на корпоративах, свадьбах, бизнес-мероприятиях по всей России и СНГ',
        second: 'Не используем фонограмму',
        third: 'Более 300 хитов в репертуаре',
      },
      carrier: {
        src: require('~/assets/img/icons/trumpet.svg'),
        alt: 'Труба'
      }
    };
  },
  methods: {
    
  },
};
</script>

<style lang="scss" scoped>
.marquee-container {
  margin-top: 30px;
  height: 30px;
  align-content: center;
  overflow: hidden;
  white-space: nowrap;
  width: 100%;
  position: relative;
  background-color: #F09014;
}

.marquee {
  display: inline-block;
  white-space: nowrap;
  animation: marquee 40s linear infinite;
  font-family: $font-subtitle;
  font-size: 16px;
  color: #000;
}

@keyframes marquee {
  0% {
    transform: translateX(0%);
  }
  100% {
    transform: translateX(-50%);
  }
}
</style>