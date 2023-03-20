<script setup lang="ts">
import Comments from "../components/Comments.vue";
</script>
<template>
  <div
    class="flex flex-row justify-between px-6 py-4 bg-amber-600 items-center text-white"
  >
    <div class="flex items-center flex-col">
      <div>
        <p class="font-bold">Frontend Mentor</p>
        <p>Feedback Board</p>
      </div>
    </div>
    <div>
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
          d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
        />
      </svg>
    </div>
  </div>
  <div class="flex justify-between px-6 py-2 bg-sky-500 text-sm text-white">
    <div class="flex flex-row items-center">
      <p>sorty by :&nbsp;</p>
      <div class="font-bold flex flex-row items-center justify-center">
        <p>Most Upvotes&nbsp;</p>
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="w-5 h-5"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M19.5 8.25l-7.5 7.5-7.5-7.5"
          />
        </svg>
      </div>
    </div>
    <button class="p-3 bg-blue-800 rounded-md font-bold">+ Add Feedback</button>
  </div>
  <Comments />
</template>
