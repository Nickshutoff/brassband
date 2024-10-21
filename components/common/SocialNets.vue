<template>
  <ul class="social-links">
    <li v-for="(icon, index) in socialIcons" :key="index">
      <a :href="icon.link" target="_blank" rel="noopener noreferrer">
        <img :src="icon.src" :alt="icon.alt">
      </a>
    </li>
  </ul>
</template>

<script>
export default {
  name: 'BrassbandSocialNets',

  data() {
    return {
      socialIcons: [
        {
          link: 'https://wa.me/',
          src: require('~/assets/img/icons/whatsapp.svg'),
          alt: 'Whatsapp'
        },
        {
          link: 'https://t.me/',
          src: require('~/assets/img/icons/telegram.svg'),
          alt: 'Telegram'
        },
        {
          link: 'https://www.youtube.com/',
          src: require('~/assets/img/icons/youtube.svg'),
          alt: 'YouTube'
        },
        {
          link: 'https://vk.com/',
          src: require('~/assets/img/icons/vk.svg'),
          alt: 'VK'
        },
      ]
    };
  },
}
</script>
<style lang="scss" scoped>
.social-links {
  display: flex;
  align-items: center;
  gap: 48px;
}
</style>