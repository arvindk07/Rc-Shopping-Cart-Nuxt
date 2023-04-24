<template>
  <div>
    <HomeWelcome />
    <!-- <button @click="toggle">Toggle</button> -->
    <component :is="Counter" />
  </div>
</template>

<script setup>
const Counter = resolveComponent("Counter");

// function toggle(){}
</script>
