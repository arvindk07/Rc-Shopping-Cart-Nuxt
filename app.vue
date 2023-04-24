<template>
  <div>
    <!-- <HomeWelcome /> -->
    <button @click="toggle">Toggle</button>
    <component :is="MyComponent" />
  </div>
</template>

<script setup>
// const MyComponent = ref(resolveComponent("Counter"));
const MyComponent = shallowRef(resolveComponent("Counter"));

function toggle() {
  MyComponent.value = resolveComponent("HomeWelcome");
}
</script>
