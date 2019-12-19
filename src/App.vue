<template>
  <div id="app">
    <!--<router-view/>-->
    <!--<SearchBar v-on:termChange="onTermChange"></SearchBar>-->
    <SearchBar @termChange="onTermChange"></SearchBar>
  </div>
</template>

<script>
import SearchBar from "./components/SearchBar";
export default {
  name: "App",
  components: {
    SearchBar
  },
  methods: {
    /*onTermChange:function(){},*/
    /* SearchBar 里面 emit 的第二个参数就是此方法的参数*/
    onTermChange(searchTerm) {
      console.log(searchTerm);
    }
  }
};
</script>

<style>
/*
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
*/
</style>
