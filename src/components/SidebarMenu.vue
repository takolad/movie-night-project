<script setup lang="ts">
import { useRouter } from "vue-router";
defineProps({
    showSidebar: Boolean
});
</script>

<template>
    <!-- class="w-screen max-w-md h-screen visisble lg:invisible bg-red-900" -->
    <div
      class="
      bg-cyan-600 text-cyan-100 w-64
      space-y-6 px-2 py-4 absolute
      inset-y-0 left-0 transform -translate-x-full
      transition duration-200 ease-in-out
      "
      :class="{ 'relative translate-x-0' : showSidebar}"
      >
      <RouterLink to="/" class="block p-4 text-center">
        <span class="text-2xl font-bold"><i class="pi pi-face-smile"></i> Movie Night</span>
      </RouterLink>
        
        <div class="flex-1">
            Calendar
        </div>
    
    </div>

</template>
