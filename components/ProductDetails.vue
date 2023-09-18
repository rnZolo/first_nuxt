<template>
    <div class="car">
        <div class="grid grid-cols-2 gap-10">
            <div class="p-7">
                <NuxtImg :src="productDetails.image" :alt="productDetails.title" />
            </div>
            <div class="p-7">
                <h1 class="text-4xl my-7">Product details for {{ productDetails.title }}</h1>
                <span class="text-xl my-7">Price - ${{ productDetails.price }}</span>
                <p class="mb-7">{{ productDetails.description }}</p>
              
               
            </div>
        </div>
    </div>
</template>

<script setup>
    const { productDetails } = defineProps(['productDetails']);
</script>

<style scoped>

</style>