<template>
  <div>
    <div>
      <button @click="increament">Increament</button>
      <h1>{{ count }}</h1>
      <button @click="decreament">Decreament</button>
    </div>
  </div>
</template>

<script setup>
const count = ref(0);

function increament() {
  count.value++;
}

function decreament() {
  count.value--;
}
</script>
