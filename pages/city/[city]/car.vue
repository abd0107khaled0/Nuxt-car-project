<template>
  <div>
    <!-- <NavBar title="cartrader" /> -->

    <div>
      <div
        class="mx-auto mt-4 max-w-7xl space-y-4 px-4 xs:px-8 sm:px-8lg:px-16 pb-16 w-3/5"
      >
        <div class="mt-32 flex">
          <div class="shadow border w-64 mr-10 z-30 h-full">
            <CarSideBar />
          </div>
          <NuxtPage />

          <!-- <CarCards /> -->
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>

const route = useRoute()

useHead({
  title: `car in ${route.params.make}`,
});

definePageMeta({
  layout:'custom',
})
</script>

<style lang="scss" scoped></style>
