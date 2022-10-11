<template>
  <div aria-live="polite">
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
}
</script>
