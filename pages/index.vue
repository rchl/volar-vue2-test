<template>
  <Tutorial/>
</template>

<script lang="ts">
export default {
  async asyncData(context) {
    context.error({message: 'err'})
  }
}
</script>
