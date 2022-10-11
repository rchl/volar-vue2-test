<template>
  <div aria-live="polite">
    <div>{{ items }}</div>
  </div>
</template>

<script>
export default {
  name: 'Index',
  props: {
    /** @type {import('vue').Prop<number[], [1, 2, 3]>} */
    items: {
      type: Array,
      default: () => [1, 2, 3]
    }
  },
}
</script>
