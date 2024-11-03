<template>
  <div>
    <div class="w-full">
      <CarCard v-for="(item, index) in 5" :key="index + Math.random()" />
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
