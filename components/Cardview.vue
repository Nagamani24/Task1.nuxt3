<template>
    <div class="card ml-3 shadow-md text-center pb-3">
        <img :src="product.image" alt="image" class="mx-auto m-2"/>
        <p class="truncate font-bold m-2">{{ product.title}}</p>
        <p>Price - ${{ product.price }}</p>
        <NuxtLink :to="`/products/${product.id}`"><p class="button mx-auto m-2">View Details</p></NuxtLink>
    </div>
</template>

<script setup>
const {product} = defineProps(['product'])
</script>

<style scoped>
img{
    max-width:400px;
    width:100px;
    height:100px;
}
.button{
    width:100px;
    height: 30px;
    text-align: center;
    background-color: aquamarine;
    border-radius:8px;
   font-size: 12px;
   padding-top:8px;
  
}
</style>