<template>
  <div>
    <div class="test" v-for="item in items">{{ item }} of {{ items.length }}</div>
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

<style scoped>
.test {
  color: red;
}
