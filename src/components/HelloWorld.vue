<script setup lang="ts">
defineProps<{
  msg: string;
}>();
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>This is the vue3 scaffold, going to become a timetracker app.</h3>
    For now it's a playground for
    <ul>
      <li>Exploring github actions</li>
      <li>Exploring tailwind css / headless ui</li>
      <li>Exploring vite / vitest</li>
      <li>Exploring scss etc. in vue builds</li>
    </ul>
  </div>
</template>

<style scoped>
li {
  margin-left: 1em;
  font-size: smaller;
}

h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
