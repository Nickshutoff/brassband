<template>
  <nav>
    <ul class="nav">
      <li v-for="(link, index) in navigationLinks" :key="index">
        <a :href="`${link.href}`">{{ link.label }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'BrassbandNavigation',

  data() {
    return {
      navigationLinks: [
        {
          label: 'Кто мы?',
          href: 'about'
        },
        {
          label: 'Фото',
          href: 'photogallery'
        },
        {
          label: 'Видео',
          href: 'videogallery'
        },
        {
          label: 'Контакты',
          href: 'contacts'
        },
      ]
    };
  },

  mounted() {
    
  },

  methods: {
    
  },
};
</script>

<style lang="scss" scoped>
  .nav {
    display: flex;
    flex-direction: row;
    gap: 56px;
  }
</style>