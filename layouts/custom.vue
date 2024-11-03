<template>
  <div>
    <h1 class="text-center text-green-500 font-bold">Custom Layout</h1>
    <!-- <p>{{ name() }}</p> -->
    <slot />
  </div>
</template>

<script setup>
import name from '~/composables/useInit';
console.log(name())
</script>

<style lang="scss" scoped></style>
