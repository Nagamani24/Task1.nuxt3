

<template>
    <div>
        <header>
            <nav class="shadow-md p-3">
                <ul class="flex gap-4">
                    <li>
                        <NuxtLink to="/">Home</NuxtLink>
                    </li>
                    <li>
                        <NuxtLink to="/products">Products</NuxtLink>
                    </li>
                    
                </ul>
            </nav>
        </header>
    </div>
    <div>
        <slot />
    </div>
</template>

<script setup>

</script>

<style scoped>
nav{
    background-color: bisque;
}
.router-link-exact-active{
    color: brown;
}
</style>