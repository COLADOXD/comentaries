<script setup lang="ts">
import { defineEmits, ref } from "vue";

const emit = defineEmits(["applyFeedback"]);
const tittle = ref("");
const comment = ref("");
const tags = ref([
  { text: "UI", isActive: true },
  { text: "UX", isActive: false },
  { text: "Enhacement", isActive: false },
  { text: "Bug", isActive: false },
  { text: "Feature", isActive: false },
]);

const onAply = () => {
  const tag = tags.value.find((tag) => tag.isActive === true);
  emit("applyFeedback", tittle, comment, tag?.text);
};

const toggleSelected = (selectedTag) => {
  tags.value.forEach((tag) => {
    if (tag.text !== selectedTag) {
      tag.isActive = false;
    } else {
      tag.isActive = true;
    }
  });
  console.log(tags.value);
};
</script>
<template>
  <div class="fixed inset-0 z-50 flex items-center justify-center">
    <div class="w-[300px] h-[400px] bg-slate-400 rounded-lg">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="w-6 h-6 flex absolute right-[50px]"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M6 18L18 6M6 6l12 12"
        />
      </svg>
      <div class="p-6">
        <p class="mb-3 font-medium text-lg">Add tittle</p>
        <input
          v-model="tittle"
          class="rounded-md px-2"
          type="text"
          placeholder="Tittle"
        />
        <p class="my-3 font-medium text-lg">Add Comment</p>
        <input
          v-model="comment"
          class="rounded-md px-2"
          type="text"
          placeholder="Comment"
        />
        <p class="my-3 font-medium text-lg">Select etiqueta</p>
        <div class="flex flex-wrap">
          <div
            v-for="(tag, index) in tags"
            :key="index"
            class="mr-3 p-1 my-2 rounded-lg"
            :class="{
              'bg-blue-600': tag.isActive,
              'bg-blue-300': !tag.isActive,
            }"
            @click="toggleSelected(tag.text)"
          >
            {{ tag.text }}
          </div>
        </div>

        <div class="flex justify-center">
          <button
            @click="onAply"
            class="bg-red-700 p-2 mt-3 rounded-lg text-white"
          >
            Add Feedback
          </button>
        </div>
      </div>
    </div>
  </div>
</template>
