<template>
  <div>
    {{ aprop  }}
    {{ foo  }}
    <Tutorial />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'
import Tutorial from '../components/Tutorial.vue'

export default Vue.extend({
  components: {
    Tutorial
  },
  props: {
    aprop: {
      type: Number,
    }
  },
  data() {
    return {
      foo: 'foo'
    }
  },
  mounted() {
    this.foo // string
  }
})
</script>
