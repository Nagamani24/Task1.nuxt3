
<template>
    <div class="m-5 p-5">
        <NuxtLink to="/products/card" class="view">Card View</NuxtLink>
        <br/>
        <br/>
        <NuxtLink to="/products/list" class="view ">List View</NuxtLink>
    </div>
</template>

<script setup>

const {data:products} = useFetch("https://fakestoreapi.com/products")

</script>

<style scoped>
.view{
    text-decoration: underline;
    color:blueviolet;
}
</style>