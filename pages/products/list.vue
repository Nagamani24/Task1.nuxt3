
<template>
    <div>
        <div v-for="product in products" class="m-4">
        
            <Listview :product="product"/>
            
        </div>
    </div>
</template>

<script setup>

const {data:products} = useFetch("https://fakestoreapi.com/products")

</script>

<style scoped>

</style>