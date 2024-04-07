<template>
    <p>HI</p>
    <EndpointItem v-for="endpoint of endpoints" :key="endpoint.id" :model="endpoint"></EndpointItem>
    <!-- <input v-model="inputText"> -->
    <!-- <button @click="endpoints.push('hi')">Add Endpoint</button> -->
  </template>
  
  <script setup>
  import { ref } from 'vue'
  import EndpointItem from './EndpointItem.vue'
  
  const endpoints = ref([
    {
        "id": 1,
        "title": "auth",
        "method": "POST"
    },
    {
        "id": 2,
        "title": "user",
        "method": "GET"
    }
  ])
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
  ul {
    text-decoration: none;
  }

  </style>
  