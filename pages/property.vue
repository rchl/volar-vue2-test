<template>
  <div>
    test
  </div>
</template>

<script>
export default {
  props: {
    items: {
      type: Boolean,
    }
  },
  computed: {
    something() {
      return this.missing
    },
  },
  data() {
    return {
      exists: true
    }
  },
}
</script>
