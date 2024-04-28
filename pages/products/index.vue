<template>
    <div>
        <div class="grid grid-cols-4 gap-5">
            <div v-for="p in products">
                <ProductCard :product="p"/>
            </div>
        </div>
    </div>
</template>

<script setup>
    import ProductCard from '/components/ProductCard.vue';
    const { data: products } = await useFetch('https://fakestoreapi.com/products');

    useHead({
        title: 'Nuxt | Products'
    })
</script>

<style>

</style>