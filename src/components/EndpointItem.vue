<template>
    <div class="endpoint"><span :class=model.method>{{ model.method }}</span> {{ model.title }}</div>
</template>

<script setup>
    defineProps({
        model: Object
    })
</script>
  
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .GET {
    background-color: green;
  }
  .POST {
    background-color: yellow;
  }
  .PUT {
    background-color: orange;
  }
</style>