<script setup lang="ts"></script>
<template>
  <div class="flex flex-row justify-between p-6 bg-amber-600 items-center">
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
  <div class="flex justify-between p-6 bg-sky-500 text-sm">
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
    <div class="p-3 bg-blue-800 rounded-md text-white font-bold">
      + Add Feedback
    </div>
  </div>
</template>
