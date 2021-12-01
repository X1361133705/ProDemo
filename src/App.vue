<template>
  <div id="app">
    <h2>-----app内容------</h2>
    <h2>{{$store.state.counter}}</h2>
    <button @click="counter++">+</button>
    <button @click="counter--">-</button>
    
    <h2>-----hellovuex内容------</h2>
    <hellovuex />
  </div>
</template>

<script>
  import hellovuex from './components/hellovuejs.vue'

  export default {
    name: 'app',
    components:{
      hellovuex
    },
    data() {
      return {
        message: '我是APP组件'
      }
    }
  }
</script>
