<template>
  <div id="app">
    <myHeader></myHeader>
    <div id="content">
      <router-view/>
    </div>
    <myFooter></myFooter>
  </div>
</template>

<script>
import myHeader from './components/myHeader.vue'
import myFooter from './components/myFooter.vue'
export default {
  name: 'App',
  components: {
    myHeader,
    myFooter
  }
}
</script>

<style>
  myHeader {
    position: fixed;
    bottom: 0;
  }
  #content {
    overflow: auto;
  }
  myFooter {
    position: fixed;
    bottom: 0;
    width: 100%;
    height: 100px;
  }
  .hello {
    height: 85vh;
    width: 100vw;
  }
</style>
