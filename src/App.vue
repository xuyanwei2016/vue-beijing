<template>
  <div id="app">
    <MHeader></MHeader>
    <Home></Home>
    <router-view/>
  </div>
</template>

<script>
  import MHeader from './components/MHeader.vue';
  import Home from './components/Home.vue';
export default {
  name: 'app',
  components:{
    MHeader,
    Home
  }
}
</script>

<style>

</style>
