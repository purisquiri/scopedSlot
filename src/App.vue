<template>
  <div id="app">
    <!-- <hello-world v-slot="v"> -->
    <hello-world #default="{ user, favorites }">
      <p>Hello {{ user.name }} you like {{ favorites[0] }}</p>
    </hello-world>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>
