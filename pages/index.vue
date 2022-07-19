<template>
  <div>
    {{ aprop  }}
    {{ foo  }}
    {{ callMeAndGetAString(1) }}
    <tutorial :test="'asdfds'" />
    <nuxt-logo></nuxt-logo>
  </div>
</template>

<script>
export default {
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
  // Uncommenting the following object makes template types work.
  // computed: {
  //   xxx() {
  //     return true;
  //   },
  // },
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
