<template>
  <div>
    <TheNav />
    <nuxt />
  </div>
</template>

<script>
import TheNav from "./partials/TheNav";
import categoriesQuery from '~/apollo/queries/category/categories';
export default {
  components: {
    TheNav
  },

  data() {
    return {
      categories: []
    };
  },

  apollo: {
    categories: {
      prefetch: true,
      query: categoriesQuery
    }
  }
};
</script>

<style>
</style>
