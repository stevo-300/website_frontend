<template>
  <div class="dream_sidebar">
    <ul>
      <li v-for="(link, i) in links" :key="i">
        <router-link :to="link.href">{{ link.title }}</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    links: [],
  },
};
</script>

<style>
.dream_sidebar {
  background-color: #b8b7b6;
  width: 100%;
  height: 100vh;
}

.dream_sidebar ul {
  position: relative;
  top: 20vh;
  text-align: right;
  padding-right: 40px;
  list-style-type: none;
}

.dream_sidebar a {
  color: white;
}

.dream_sidebar a:hover {
  color: white;
  text-decoration: none;
}
</style>
