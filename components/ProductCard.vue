
import { NuxtLink } from '#build/components';

import { NuxtLink } from '#build/components';

import productsVue from '~/layouts/products.vue';

import productsVue from '~/layouts/products.vue';
<template>
    <div class="card text-center flex flex-col">
        <h2 class="card-title font-bold text-gray-500 m-4 truncate">{{ product.title }}</h2>
        <NuxtImg :src="`${product.image}`" alt="{{ product.title }}" srcset="" class="product-image"/>
            <span>{{ product.price }}</span>
        <NuxtLink :to="`/products/${product.id}`" class="btn min-w-[200px]">View</NuxtLink>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product']);
</script>

<style lang="scss" scoped>

</style>