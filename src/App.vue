<template>
  <Home />
</template>

<script>
import Home from "./pages/home.vue";

export default {
  name: "App",
  components: {
    Home,
  },
};
</script>
<style lang="scss" scoped>
#app {
  display: flex;
  flex-direction: column;
}
</style>