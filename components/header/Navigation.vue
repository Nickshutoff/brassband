<template>
    <ul class="navigation-links">
      <li v-for="(link, index) in navigationLinks" :key="index">
        <a :href="`${link.href}`">{{ link.label }}</a>
      </li>
    </ul>
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
}
</script>

<style lang="scss" scoped>
  .navigation-links {
    display: flex;
    align-items: center;
    gap: 56px;
  }
</style>