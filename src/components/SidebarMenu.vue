<script setup>
import { ref } from 'vue'
const open = ref(true)
</script>

<template>
    <div class="w-screen max-w-md h-screen visisble lg:invisible bg-red-900">
        <div class="text-right">
            <button @click="open = false"><i class="bx bx-user"></i></button>
        </div>
        This is just a test
    </div>
</template>