<template>
  <h4 class="section-heading">{{ heading }}</h4>
</template>

<script>
export default {
  name: 'BrassbandHeadingComponent',

  props: {
    heading: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.section-heading {
  font-family: $font-title;
  font-size: 48px;
}
</style>