<template>
  <div aria-live="polite">
    <div class="some-class">{{ computedProp }}</div>
    <div>{{ items }}</div>
  </div>
</template>

<script>
export default {
  name: 'Index',
  props: {
    /** @type {import('vue').PropOptions<number[]>} */
    items: {
      type: Array,
      default: () => [1, 2, 3]
    }
  },
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
