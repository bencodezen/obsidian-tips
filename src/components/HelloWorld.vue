<script setup lang="ts">
defineProps<{
  msg: String
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="purple">{{ msg }}</h1>
    <p class="subtitle">
      A site dedicated to provided tips and tricks for getting the most out of
      <a href="https://obsidian.md/">Obsidian</a>.
    </p>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

.subtitle {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    display: block;
    text-align: left;
  }
}
</style>
