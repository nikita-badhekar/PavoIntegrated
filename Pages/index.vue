<template>
  <div class="bg-gray-900 text-white flex justify-evenly">
    <NuxtLink to="/">Index Page</NuxtLink>
    <NuxtLink to="/newPage">  Theme </NuxtLink>
    <NuxtLink to="/article">Article</NuxtLink>
    <NuxtLink to="/privacy">Privacy</NuxtLink>
    <NuxtLink to="/terms">Terms</NuxtLink>
  </div>
</template>

<script>
import { reactive, toRefs } from "vue";

export default {
  setup() {
    const state = reactive({
      count: 0,
    });

    return {
      ...toRefs(state),
    };
  },
};
</script>

<style lang="scss" scoped>

</style>
