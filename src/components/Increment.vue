<template>
    <button @click="increment">Increment</button>
  </template>
  
  <script>
  export default {
    methods: {
      increment() {
        this.$emit("increment");
      }
    }
  };
  </script>
  
  <style scoped>
  button {
    font-size: 20px;
    padding: 10px;
    margin: 5px;
    cursor: pointer;
  }
  </style>
  