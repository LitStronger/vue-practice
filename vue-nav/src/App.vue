<template>
  <div id="app">
    <myNav />
    <!-- <list /> -->
    <!-- <vModelTest msg="init" /> -->
  </div>
</template>
<script>
import myNav from './components/myNav'
// import list from './components/v-for.vue'
// import vModelTest from './components/v-model'
export default {
  name: 'App',
  components: {
    // list,
    // vModelTest,
    myNav
  }
}
</script>

<style>
body{
  margin: 0;
  padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
