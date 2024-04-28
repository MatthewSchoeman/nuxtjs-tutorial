<template>
    <div class="card text-center">
        <img :src=product.image alt="product thmb" class="mx-auto my-7">
        <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
        <nuxt-link :to="`/products/${product.id}`">
            <p class="btn">View Details</p>
        </nuxt-link>
    </div>
</template>

<script setup>
    const { product } = defineProps(['product']);
    // console.log(product.id);
</script>

<style scoped>
    img {
        max-height: 150px;
    }
</style>