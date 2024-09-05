<script setup>

defineProps({
    image: String,
    title: String,
})

</script>

<template>
    <div class=" hover:bg-gray-100 cursor-pointer mb-3">
        <div class="flex items-center gap-3 py-2 px-2">

            <img :src="image" alt="" class="w-[32px] rounded-full">
        <div>
            <h3 class="font-black">{{ title }}</h3>
        </div>
        </div>
    </div>
</template>