<template>
  <div>
    {{ aprop  }}
    {{ foo  }}
    {{ callMeAndGetAString(1) }}
    <Tutorial :test="'asdfds'" />
  </div>
</template>

<script>
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
  methods: {
    /**
     * @param {number} arg
     * @return {string}
     */
    callMeAndGetAString(arg) {
      return String(arg) + 'xxx';
    }
  },
  mounted() {
    this.foo // string
  }
})
</script>
