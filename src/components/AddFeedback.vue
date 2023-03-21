<template>
  <div class="fixed inset-0 z-50 flex items-center justify-center">
    <div class="w-[300px] h-[400px] bg-slate-400 p-6 rounded-lg">
      <p class="mb-3 font-medium text-lg">Add tittle</p>
      <input type="text" placeholder="Tittle" />
      <p class="my-3 font-medium text-lg">Add Comment</p>
      <input type="text" placeholder="Comment" />
      <p class="my-3 font-medium text-lg">Select etiqueta</p>
      <div class="flex flex-wrap">
        <div class="bg-blue-300 mr-3 p-1 my-2 rounded-lg">All</div>
        <div class="bg-blue-300 mr-3 p-1 my-2 rounded-lg">UI</div>
        <div class="bg-blue-300 mr-3 p-1 my-2 rounded-lg">UX</div>
        <div class="bg-blue-300 mr-3 p-1 my-2 rounded-lg">Enhacement</div>
        <div class="bg-blue-300 mr-3 p-1 my-2 rounded-lg">Bug</div>
        <div class="bg-blue-300 mr-3 p-1 my-2 rounded-lg">Feature</div>
      </div>
    </div>
  </div>
</template>
