
<template>
    <div>
        <header>
            <nav class="flex p-3">
                <div class="flex gap-4">
                    <NuxtLink to="/">Home</NuxtLink>
                    <NuxtLink to="/products">Poducts</NuxtLink>
                </div>
               <div class="ml-auto">
                <button>Buy Product</button></div>
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
    background-color: #e4f2eb;
}
button{
      font-size: 12px;
      background-color: #5891ed;
      width:100px;
      height: 30px;
      border-radius: 8px;
      text-align: center;
      color: white;
      padding:5px;
     
      margin: auto;
}


</style>