<script setup lang="ts">
import TopBar from "@/components/TopBar.vue";
import SidebarMenu from "@/components/SidebarMenu.vue";
import { ref } from "vue";

const showSidebar = ref(false);
const toggleSidebar = () => {
  showSidebar.value = !showSidebar.value;
};
</script>

<template>
  <main class="relative flex"
    style="margin-top: 56px; min-height: calc(100vh - 56px);">
    <TopBar :toggleSidebar="toggleSidebar" />
    <SidebarMenu :showSidebar="showSidebar" />
  </main>
</template>
