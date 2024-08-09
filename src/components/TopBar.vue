<script setup lang="ts">

const props = defineProps({
    toggleSidebar: Function
});
</script>

<template>
    <div class="flex-1 absolute top-0 w-full" style="margin-top: -56px;">
        <div class="bg-white shadow px-2 py-4">
            <button @click="props.toggleSidebar" class="px-2">
                <i class="pi pi-bars"></i>
            </button>
        </div>
    </div>
</template>