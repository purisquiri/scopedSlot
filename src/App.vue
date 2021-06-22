<template>
  <div id="app">
    <!-- <hello-world v-slot="v"> -->
    <hello-world #default="{ user, favorites }">
      <p>Hello {{ user.name }} you like:</p>
      <ul>
        <li v-for="favorite in favorites" :key="favorite">{{ favorite }}</li>
      </ul>
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
