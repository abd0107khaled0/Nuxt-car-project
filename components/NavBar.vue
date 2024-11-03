<template>
  <div>
    <header
      class="sticky top-0 z-50 flex justify-between items-center space-x-1 border-b bg-white p-4 shadow-md"
    >
      <!-- <a href="/" class="text-3xl font-mono">
        {{ title }}
      </a> -->

      <!-- <NuxtLink to="/" class="text-3xl font-mono"> {{ title }}</NuxtLink> -->
      <NuxtLink :to="{path:'/', query:{form:$route.name} }" class="text-3xl font-mono"> {{ title }}</NuxtLink>
    </header>
  </div>
</template>

<script setup>
const propsHeader = defineProps(["title"]);
</script>

<style lang="scss" scoped></style>
