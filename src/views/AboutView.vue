<script setup lang="ts">
import { sum, divide, multiply, subtract } from 'procgen'
</script>

<template>
  <div class="about">
    <div>
      <h1>This is an about page</h1>

      <p>Let's do some math... with wasm!</p>
      <p>1 + 2 = {{ sum(1, 2) }}</p>
      <p>1 - 2 = {{ subtract(1, 2) }}</p>
      <p>1 * 2 = {{ multiply(1, 2) }}</p>
      <p>6 / 2 = {{ divide(6, 2) }}</p>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
