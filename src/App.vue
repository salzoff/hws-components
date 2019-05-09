<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import FormDataRequest from '@salzoff/hwsclient/src/classes/request/FormDataRequest';
export default {
    name: 'app',
    components: {
        HelloWorld
    },
    mounted() {
      const request = new FormDataRequest();
      console.log(request.getOwnProperties());
    }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
