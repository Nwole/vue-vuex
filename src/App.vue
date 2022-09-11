<template>
  <v-app>
    <div class="container">
      <h1>Vuex</h1>
      <Result />
      <AnotherResult />
      <Counter />
      <AnotherCounter/>
    </div>
    <v-main>
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import Counter from "./components/Counter.vue";
import Result from "./components/Result.vue";
import AnotherResult from "./components/AnotherResult.vue";
import AnotherCounter from "./components/AnotherCounter.vue";

export default {
  name: "App",
  data() {
    return {};
  },
  components: { Counter, Result, AnotherResult, AnotherCounter },
};
</script>
<style scoped>
.container {
  width: 80%;
  margin: auto;
}
</style>
