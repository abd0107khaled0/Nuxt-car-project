<template>
  <div>
    <NuxtLink to="/car/car-1">
      <div
        class="shadow border w-full overflow-hidden mb-5 cursor-pointer h-[200px]"
      >
        <div class="flex h-full">
          <img src="/public/splashpage.jpg" alt="car" class="w-300px h-full" />
          <div class="p-4 flex flex-col">
            <div>
              <h1 class="text-2xl text-blue-700 capitalize">volvo XC0</h1>
              <p class="text-gray-700">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Dignissimos, a. Qui amet architecto tenetur, porro ad
              </p>
            </div>
            <h1 class="mt-auto text-xl">$39,555</h1>
          </div>
        </div>
      </div>
    </NuxtLink>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
