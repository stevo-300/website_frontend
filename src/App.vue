<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-sm">
          <Sidebar :links="links" />
        </div>
        <div class="col">
          <router-view />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import Navbar from "./components/common/navbar.vue";
import Sidebar from "./components/common/sidebar.vue";

export default {
  data() {
    return {
      links: [
        {
          href: "/",
          title: "Blog",
        },
        {
          href: "/about",
          title: "About",
        },
        {
          href: "/categories",
          title: "Categories",
        },
        {
          href: "/projects",
          title: "Projects",
        },
      ],
    };
  },
  components: {
    // Navbar,
    Sidebar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.container {
  padding: 0;
  max-width: 100vw;
  overflow-x: hidden;
}

.container .col-sm {
  max-width: 30%;
}

.container .col {
  padding-right: 25px;
}
</style>
