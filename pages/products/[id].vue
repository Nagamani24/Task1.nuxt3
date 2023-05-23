
<template>
    <div class="p-5">
        <div class="mt-4">
        <Productdetails :product="product"/>
    </div>
    </div>
</template>


<script setup>


    const {id} = useRoute().params

    const uri = "https://fakestoreapi.com/products/"+id

    const {data:product} = await useFetch(uri)
    
    definePageMeta({
    layout:'prolay'
})

</script>


<style scoped>

</style>