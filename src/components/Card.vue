<template>
  <div class="card">
    <header class="card-header">
      <slot name="header" />
    </header>

    <main class="card-body">
      <slot />
    </main>

    <footer class="card-footer">
      <slot name="footer" />
    </footer>
  </div>
</template>

<script setup>
</script>

<style scoped>
.card {
  border: 1px solid #ccc;
  padding: 1rem;
  border-radius: 10px;
  margin-bottom: 1rem;
  background: #fefefe;
}
.card-header,
.card-footer {
  background: #eee;
  padding: 0.5rem;
  font-weight: bold;
}
.card-body {
  padding: 1rem 0;
}
</style>
