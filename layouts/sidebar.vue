<template>
  <main class="user-layout">
    <article class="sidebar">
      <p>dashboard</p>
      <p>setting</p>
    </article>
    <section>
      <!-- here nuxt will replace page content -->
      <slot></slot>
    </section>
  </main>
</template>

<style>
.sidebar {
  display: flex;
  flex-direction: column;
}
.user-layout {
  display: flex;
}
</style>
