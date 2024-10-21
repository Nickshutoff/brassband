<template>
  <button class="button">{{text}}</button>
</template>

<script>
export default {
  name: 'BrassbandButtonTemplate',

  props: {
    text: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.button {
  width: 266px;
  height: 60px;
  font-family: $font-primary;
  font-size: 20px;
  border-radius: 20px;
  color: var(--transparent); //Need to be redone
  background-color: var(--c-600);
}
</style>