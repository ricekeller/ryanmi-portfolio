<template>
    <div class="bg-white dark:bg-gray-900 rounded-lg shadow-md overflow-hidden">
        <img class="w-full h-34 object-cover" :src="imageUrl" alt="Card Image">
        <div class="p-6 ">
            <h2 class="text-xl font-semibold">{{ title }}</h2>
            <p class="text-gray-600">{{ description }}</p>
        </div>
    </div>
</template>

<script setup>


defineProps({
    title: String,
    description: String,
    imageUrl: String
});

</script>