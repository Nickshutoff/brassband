<template>
  <div class="about-text-content">
    <p>{{text.first}}</p>
    <p>{{text.second}}</p>
  </div>
</template>

<script>
export default {
  name: 'BrassbandAboutText',

  data() {
    return {
      text: {
        first: 'Большая и зрелищная музыкальная банда из восьми лихих гусаров. В нашем арсенале имеются: труба, сакс, валторна, тромбон, туба, ударные, гитара и вокал.',
        second: 'Группа на сцене — это мы. Лаунж для коктейльной вечеринки — это мы. Марширующий оркестр — снова мы.'
      }
    };
  },
};
</script>

<style lang="scss" scoped>
.about-text-content {
  font-family: $font-primary;
  color: var(--c-600);
}
</style>