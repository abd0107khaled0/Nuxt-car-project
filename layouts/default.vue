<template>
    <div>
     <!-- <NavBar title="Carrader layout"/> -->
     <div class="text-center">
        <p class="text-green-500 font-bold">
            Layout
        </p>
     </div>
     <slot />
    </div>
  </template>
  
  <script setup>
  const propsHeader = defineProps(["title"]);
  </script>
  
  <style lang="scss" scoped></style>
  