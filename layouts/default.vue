<template>
    <div>
        <header class="shadow-sm bg-white">
            <nav class="container mx-auto p-4 flex justify-between">
                <nuxt-link to="/" class="font-bold">Logo Here</nuxt-link>
                <ul class="flex gap-4">
                    <li><nuxt-link to="/">Home</nuxt-link></li>
                    <li><nuxt-link to="/about">About</nuxt-link></li>
                    <li><nuxt-link to="/products" class="btn">Products</nuxt-link></li>
                </ul>
            </nav>
        </header>
    </div>

    <div id="body">
        <div class="container mx-auto p-4" id="body">
            <slot />
        </div>
    </div>
</template>

<style>
    .router-link-exact-active { 
        color: #12b488;
    }

    #body { 
        background-image: url("assets/images/about1.png");
        background-repeat: no-repeat;
        background-size: 100% 100%;
    }
</style>