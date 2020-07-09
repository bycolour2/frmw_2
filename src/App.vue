<template>
  <div id="app">
    <div>
      <input v-model="count" />
      <input v-model="text" />
    </div>
    <div>
      <template v-for="i in +count">
        <input :value="text" v-bind:key="i" />
      </template>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      count: "",
      text: "",
    }
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
  margin-top: 60px;
}
</style>
