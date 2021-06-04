<template>
  <div id="app">
    <p class="dd">hello {{ msg }}</p>

    <vuea />
    <vueb />
  </div>
</template>

<script>
import vuea from "./components/vue1.vue";
import vueb from "./components/vue2.vue";
export default {
  name: "app",
  data() {
    return {
      msg: "vue.js",
    };
  },
  components: {
    vuea,
    vueb,
  },
};
</script>

<style scoped>
.dd {
  color: red;
}
</style>
