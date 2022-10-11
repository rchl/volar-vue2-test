<template>
  <div aria-live="polite">
    <div class="some-class">{{ computedProp }}</div>
  </div>
</template>

<script>
export default {
  name: 'Index',
  computed: {
    computedProp() {
      return 'foo'
    },
  },
}
</script>

<style scoped>
.some-class {
  color: blue;
}
</style>
