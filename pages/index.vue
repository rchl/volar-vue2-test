<template>
  <div>
    <div class="test" v-for="item in items">{{ item }} of {{ items.length }}</div>
  </div>
</template>

<script>
export default {
  name: 'Index',
  props: {
    items: {
      /** @type {import('vue').PropType<number[]>} */
      type: Array,
      default: () => [1, 2, 3]
    }
  },
  computed: {
    foo() {
      return this.xxx
    },
  },
}
</script>

<style scoped>
.test {
  color: red;
}
