<template>
  <div class="blog_article">
    <b-card no-body>
      <!-- <template #header>
        <h4 class="mb-0">Hello World</h4>
      </template> -->

      <b-card-body>
        <b-card-title>{{ article.title }}</b-card-title>
        <!-- <b-card-sub-title class="mb-2">Card Sub Title</b-card-sub-title> -->
        <b-card-text>
          {{ article.snippet }}
        </b-card-text>
      </b-card-body>

      <b-list-group flush>
        <b-list-group-item>Categories</b-list-group-item>
        <b-list-group-item>{{ article.datePosted }}</b-list-group-item>
      </b-list-group>
    </b-card>

    <!-- <b-card
      :title="article.title"
      tag="article"
      style="max-width: 20rem"
      class="mb-2"
    >
      <b-card-text>
        {{ article.snippet }}
      </b-card-text>
    </b-card> -->
  </div>
</template>

<script>
export default {
  props: {
    article: {},
  },
};
</script>

<style>
.card {
  border: none;
  text-align: left;
}

.card: n;
</style>
