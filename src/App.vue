<template>
  <div id="app">
    <MyHeader />
    <ItemGrid />
    <MyFooter />
  </div>
</template>

<script>
  import MyHeader from './components/MyHeader.vue';
  import MyFooter from './components/MyFooter.vue';
  import ItemGrid from './components/ItemGrid.vue';
  
  export default {
    name: 'App',
    
    components:{
      MyHeader,
      ItemGrid,
      MyFooter
    }
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height: 100vh;
  position: relative;
}
</style>
