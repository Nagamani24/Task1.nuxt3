

<template>
    <div class = "grid grid-cols-2">
        <div class="p-4 mx-auto my-7 shadow-md">
            <img :src="product.image" alt="img"/>
        </div>
        <div class="p-4 shadow-md">
            <p class="text-4xl m-4">{{ product.title }}</p>
            <p class="text-2xl m-4">Price - ${{ product.price }}</p>
            <p class="text-3xl mt-7 ml-4">Product Description</p>
            <hr/>
            <p class="m-4">{{ product.description }}</p>
        </div>
    </div>
   
</template>


<script setup>
const {product} = defineProps(['product'])

</script>


<style scoped>
img{
    width: 400px;
    height: 400px;
    max-width: 400px;
   
}
</style>