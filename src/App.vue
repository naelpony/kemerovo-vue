<template>
  <header>
    <head-search />
    <head-menu />
  </header>
</template>
<script>
import HeadMenu from "./components/HeadMenu.vue";
import HeadSearch from "./components/HeadSearch.vue";


export default {
  components: {
    HeadSearch,
    HeadMenu,
  },
};
</script>
