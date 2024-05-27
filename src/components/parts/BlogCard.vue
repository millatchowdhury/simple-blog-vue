<script setup>
defineProps({
    post: Object,
});
</script>

<template>
    <router-link :to="`/blog/${post.id}`">
<div class="max-w-md rounded overflow-hidden shadow-lg">
      <img
        class="w-full"
        src="https://images.unsplash.com/photo-1614082242765-7c98ca0f3df3?q=80&w=2070&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
        alt="Sunset in the mountains"
      />
      <div class="px-6 py-4">
        <div class="font-bold text-xl mb-2">{{ post.title }}</div>
        <p class="text-gray-700 text-base">
          {{ post.body }}
        </p>
      </div>
      <div class="px-6 pt-4 pb-2">
        <span
        v-for="tag in post.tags" :key="tag"
        class="inline-block bg-gray-200 rounded-full px-3 py-1 text-sm font-semibold text-gray-700 mr-2 mb-2">
          {{ tag  }}
        </span>
       
     
      </div>
    </div>
</router-link>
</template>

<style scoped>

</style>