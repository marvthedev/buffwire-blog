<template>
  <div class="blog">
    <div v-for="articles in articles" :key="articles.id" class="blog__post">   
        <h2>{{ articles.title }}</h2>
        <p>{{ articles.excerpt }}</p>
    </div>
  </div>
</template>

<script>
import articlesQuery from "~/apollo/queries/article/articles";
import categoriesQuery from "~/apollo/queries/category/categories";

export default {
  apollo: {
    articles: {
      prefetch: true,
      query: articlesQuery
    },

    categories: {
      prefetch: true,
      query: categoriesQuery
    }
  }
};
</script>
