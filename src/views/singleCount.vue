<template>
    <div class="counter-container">
      <!-- Decrement Button -->
      <button @click="decrementCounter">-</button>
      
      <!-- Counter Display -->
      <div class="counter">{{ count }}</div>
      
      <!-- Increment Button -->
      <button @click="incrementCounter">+</button>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        count: 0  // Initial count value
      };
    },
    methods: {
      // Method to increment the counter
      incrementCounter() {
        this.count++;
      },
      // Method to decrement the counter
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
    font-size: 40px;
    margin: 0 20px;
    color: darkmagenta;
  }
  
  button {
    font-size: 20px;
    padding: 10px;
    margin: 5px;
    cursor: pointer;
    background-color: aqua;
  }
  </style>
  