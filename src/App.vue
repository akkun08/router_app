<template>
  <div id="app">
    <div>
      <router-link
        :to="{ name: 'index', params: { name: 'TARO' } }"
        class="btn btn-primary mx-2"
      >
        Go to Top
      </router-link>
      <router-link
        :to="{ name: 'index', params: { name: 'HANAKO' } }"
        class="btn btn-warning"
      >
        Go to JSX
      </router-link>
    </div>
    <hr />
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: "app",
  created() {
    console.log("***** App Created! *****");
  },
  mounted() {
    console.log("----- App Mounted! -----");
  },
  data() {
    return {
      title: "Router",
    };
  },
};
</script>