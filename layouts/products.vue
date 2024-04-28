<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <nuxt-link to="/products" class="font-bold btn">Back To Products</nuxt-link>
                
            </nav>
        </header>
    </div>

    <div class="container mx-auto p-4">
        <slot />
    </div>

    <footer class="container mx-auto p-4">
        <ul class="flex gap-4">
            <li><nuxt-link to="/">Home</nuxt-link></li>
            <li><nuxt-link to="/products">Products</nuxt-link></li>
            <li><nuxt-link to="/about">About</nuxt-link></li>
        </ul>
    </footer>
</template>