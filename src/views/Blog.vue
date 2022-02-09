<template>
  <div class="blogroll">
    <BlogListArticle
      v-for="article in articles"
      :key="article.id"
      :article="article"
      class="blog-article"
    ></BlogListArticle>
  </div>
</template>

<script>
import BlogListArticle from "../components/blog/listArticle.vue";
export default {
  data() {
    return {
      articles: [
        {
          title: "Blog",
          snippet: "Blah di blah di blah 1",
          datePosted: "29/1/2022",
          categories: ["tech", "code", "flutter"],
          id: 1,
        },
        {
          title: "About",
          snippet: "Blah di blah di blah 1",
          datePosted: "29/1/2022",
          categories: ["tech", "code", "javascript"],
          id: 2,
        },
        {
          title: "Categories",
          snippet: "Blah di blah di blah 1",
          datePosted: "29/1/2022",
          categories: ["tech", "business central"],
          id: 3,
        },
        {
          title: "Projects",
          snippet: "Blah di blah di blah 1",
          datePosted: "29/1/2022",
          categories: ["recipes"],
          id: 4,
        },
      ],
    };
  },
  components: {
    BlogListArticle,
  },
};
</script>

<style>
.blog-article:not(:first-child) {
  margin-top: 5vh;
}
</style>
