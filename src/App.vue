<template>
  <div class="antialiased">
    <div class="relative bg-gray-200">
      <div class="absolute inset-0 flex flex-col" aria-hidden="true">
        <div class="flex-1 bg-gray-100"></div>
        <div class="flex-1 bg-gray-200"></div>
      </div>
      <div class="relative max-w-main mx-auto">
        <div class="flex flex-col min-h-screen lg:flex-row lg:items-center">
          <div
            class="flex flex-col flex-grow my-8 py-6 bg-white lg:shadow-2xl lg:rounded-lg lg:overflow-hidden"
          >
            <h2 class="text-center text-2xl font-bold mb-2">SEASON SPONSOR</h2>
            <div class="customGrid tier1 mb-6">
              <span v-for="i in 4" :key="'tier1' + i">
                <img src="./images/tier1.png" alt="Logo tier1" srcset="" />
              </span>
            </div>

            <h2 class="text-center text-2xl font-bold mb-2">SUPPORTING SPONSOR</h2>
            <div class="customGrid tier2 mb-6">
              <span v-for="i in 10" :key="'tier2' + i">
                <img src="./images/tier2.png" alt="Logo tier2" srcset="" />
              </span>
            </div>

            <h2 class="text-center text-2xl font-bold mb-2">COMMUNITY SPONSOR</h2>
            <div class="customGrid tier3 mb-6">
              <span v-for="i in 10" :key="'tier3' + i">
                <img src="./images/tier3.png" alt="Logo tier3" srcset="" />
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
};
</script>

<style>
.customGrid {
  display: grid;
  gap: 16px;
  justify-content: space-evenly;
}

.tier1 {
  grid-template-columns: repeat(auto-fill, 300px);
}

.tier2 {
  grid-template-columns: repeat(auto-fill, 240px);
}

.tier3 {
  grid-template-columns: repeat(auto-fill, 180px);
}
</style>
