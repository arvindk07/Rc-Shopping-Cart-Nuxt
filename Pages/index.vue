<template>
  <button @click="moveToAbout">Take me to About Page</button>
  Hello Index
</template>

<script setup>
function moveToAbout() {
  navigateTo("about");
}
</script>
