<template>
    <button @click="sendMessage">Send Message to Parent</button>
  </template>
  
  <script>
  export default {
    methods: {
      sendMessage() {
        this.$emit('message-from-child', 'Hello from Child!');
      }
    }
  }
  </script>
  