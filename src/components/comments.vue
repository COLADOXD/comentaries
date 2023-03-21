<script setup lang="ts">
console.log("hola");
</script>
<template>
  <div class="px-6 py-6">
    <div class="bg-white p-6 flex flex-col rounded-xl">
      <p class="font-bold">Add tags for solutions</p>
      <p class="my-2">Easir to search for solutions on a specific stack.</p>
      <button
        class="flex justify-start px-3 p-2 mt-4 bg-gray-200 w-[90px] rounded-lg text-blue-600 font-bold"
      >
        Etiqueta
      </button>
      <div class="flex justify-between mt-4">
        <div class="flex items-center p-2 rounded-lg bg-slate-200">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-4 h-4"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M4.5 15.75l7.5-7.5 7.5 7.5"
            />
          </svg>
          <p class="font-bold ml-2">100</p>
        </div>
        <div class="flex items-center p-2">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            fill="none"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="currentColor"
            class="w-6 h-6"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              d="M12 20.25c4.97 0 9-3.694 9-8.25s-4.03-8.25-9-8.25S3 7.444 3 12c0 2.104.859 4.023 2.273 5.48.432.447.74 1.04.586 1.641a4.483 4.483 0 01-.923 1.785A5.969 5.969 0 006 21c1.282 0 2.47-.402 3.445-1.087.81.22 1.668.337 2.555.337z"
            />
          </svg>
          <p class="font-bold ml-2">2</p>
        </div>
      </div>
    </div>
  </div>
</template>
