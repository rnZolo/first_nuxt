<template>
  <div>
    <ProductDetails :productDetails="productDetails"/>
  </div>
</template>

<script setup>
  const { id } = useRoute().params;
  const { data: productDetails } = await useFetch(`https://fakestoreapi.com/products/${id}`, {key: id});
  console.log(product);
  definePageMeta({
    layout: "products",
  })
</script>