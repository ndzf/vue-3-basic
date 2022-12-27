<template>
  <h1>{{ message }}</h1>
  <span title="static value">Hover me (without declarative rendering)</span>
  <br>
  <span :title="message">Hover me (with declarative rendering)</span>
  <br>
  <button @click="changeMessage">Change message</button>
</template>

<script>
/**
 * Declarative rendering: vue extends standard HTML with template syntax that allows us to declaratively 
 * describe HTML output based on javascript state.
 * source: https://vuejs.org/guide/introduction.html#what-is-vue
 */
export default {
  data() {
    return {
      message: "Declarative rendering",
    }
  },
  methods: {
    changeMessage(e) {
      this.message = "Hello world";
    }
  }
}
</script>