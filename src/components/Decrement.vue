<template>
    <button @click="decrement">Decrement</button>
  </template>
  
  <script>
  export default {
    methods: {
      decrement() {
        this.$emit("decrement");
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
  