<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <div>
    {{ animal }}
  </div>
  <div>Monkey likes {{ food }}</div>
  <input type="text" v-model="food" />
  <div v-html="alertMessage"></div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      animal: "monkey",
      food: "apple",
      alertMessage: "<h2>Alert</h2>",
    };
  },
  components: {},
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
input {
  font-size: 15px;
}
</style>
