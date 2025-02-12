<template>
    <div class="counter-container">
      <Decrement @decrement="decrementCounter" />
      <div class="counter">{{ count }}</div>
      <Increment @increment="incrementCounter" />
    </div>
  </template>
  
  <script>
  import Increment from '@/components/Increment.vue';
  import Decrement from '@/components/Decrement.vue';
  
  export default {
    components: {
      Increment,
      Decrement
    },
    data() {
      return {
        count: 0
      };
    },
    methods: {
      incrementCounter() {
        this.count++;
      },
      decrementCounter() {
        this.count--;
      }
    }
  };
  </script>
  
  <style scoped>
  .counter-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
  }
  
  .counter {
    font-size: 50px;
    margin: 0 20px;
  }
  
  button {
    font-size: 20px;
    padding: 10px;
    margin: 5px;
    cursor: pointer;
  }
  </style>
  