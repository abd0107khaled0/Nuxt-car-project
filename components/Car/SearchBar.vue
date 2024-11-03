<template>
  <div>
    <div
      class="font-serif w-[1000px] text-2xl rounded-full bg-white flex justify-between overflow-hidden drop-shadow-2xl mx-auto"
    >
      <input
        type="text"
        class="py-3 px-5 w-full text-2xl rounded-full focus:outline-none"
        placeholder="Search by city..."
        v-model="city"
      /> 
      <button
        class="bg-sky-500 px-10 text-white"
        @click="handleSearch"
        :class="cityError ? 'border-2 border-rose-500' : ''"
        :style="[cityError?'border-radius:0 26px 26px 0':'']"
      >
        Search
      </button>
    </div>
  </div>
</template>

<script setup>
// import
import { ref } from "vue";

// ref & reactive
const city = ref("");
const cityError = ref(false);

const router = useRouter();
const route = useRoute();

// methods
const handleSearch = () => {
  if (city.value.trim()) {
    navigateTo(`city/${city.value}/car`);
  } else return (cityError.value = true);

  // router.push(`city/${city.value}/car`);
};
// console.log
// console.log(router);
</script>

<style lang="scss" scoped></style>
