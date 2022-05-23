<template>
  <div>
    {{ aprop  }}
    {{ foo  }}
    {{ callMeAndGetAString(1) }}
    <Tutorial :test="'asdfds'" />
  </div>
</template>

<script>
import Tutorial from '../components/Tutorial.vue'

export default {
  components: {
    Tutorial
  },
  props: {
    aprop: {
      type: Number,
    }
  },
  async asyncData(context) {
    context.redirect('https://google.com');
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
}
</script>
