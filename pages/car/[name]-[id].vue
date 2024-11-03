<template>
  <div>
    <NavBar title="careader" />

    <div>
      <div
        class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-10 lg:px-16 pb-1"
      >
        <!-- car hero -->
        <CarDetails />
        <!-- car hero -->

        <!-- car attributes -->
        <CarAttributes />
        <!-- car attributes -->

        <!-- description -->
        <CarDescription />
        <!-- description -->

        <!-- contact  -->
        <CarContact />
        <!-- contact  -->
      </div>
    </div>
  </div>
</template>

<script setup>
import { inject } from "vue";
const injectApp = inject("route");

useHead({
  title: injectApp.name.split("-").join(" ").toUpperCase(),
});
</script>

<style lang="scss" scoped></style>
