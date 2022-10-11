<template>
  <div aria-live="polite">
    <div>{{ computedProp }}</div>
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
