<template>
  <div>
    <!-- <HomeWelcome /> -->
    <button @click="toggle">Toggle</button>
    <!-- <component :is="MyComponent" /> -->
    <div v-if="MyComponent === 'welcome'">
      <HomeWelcome />
    </div>
    <Counter v-else />
  </div>
</template>

<script setup>
// const MyComponent = ref(resolveComponent("Counter"));
const MyComponent = ref("counter");

function toggle() {
  MyComponent.value = "welcome";
}
</script>
