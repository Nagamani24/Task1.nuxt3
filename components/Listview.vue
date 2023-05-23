

<template>
    <div class="card truncate ml-3">
        <ul>
            <li class="list-style"><NuxtLink>{{ product.title}}</NuxtLink></li>
        </ul>
       
        
        
    </div>
</template>

<script setup>
const {product} = defineProps(['product'])
</script>

<style scoped>
.list-style{
    list-style-type: none;
}
</style>