
<template>
    <div class="grid grid-cols-3 gap-3">
        <div v-for="product in products" class="m-4">
        
            <Cardview :product="product"/>
            
        </div>
    </div>
</template>

<script setup>

const {data:products} = useFetch("https://fakestoreapi.com/products")

</script>

<style scoped>

</style>