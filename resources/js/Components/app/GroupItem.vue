<script setup>

defineProps({
    image: String,
    title: String,
    description: String,
})

</script>

<template>
    <div class=" hover:bg-gray-100 cursor-pointer mb-3">
        <div class="flex items-start gap-1 py-2 px-2">

            <img :src="image" alt="" class="w-[32px] rounded-full">
        <div>
            <h3 class="font-black text-xl">{{ title }}</h3>
            <p class="text-xs text-gray-400"> {{ description }}</p>
        </div>
        </div>
    </div>
</template>