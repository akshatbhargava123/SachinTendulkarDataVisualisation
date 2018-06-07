<template>
  <div id="app">
    <Content />
  </div>
</template>

<script>
import Content from "./components/Content.vue";

export default {
  name: "app",
  components: {
    Content
  },
  mounted() {
    this.$vs.loading();
    setTimeout(() => {
      this.$vs.loading.close();
    }, 2000);
  }
};
</script>

<style>
</style>
