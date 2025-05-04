<template>

<section class="categories py-[120px] px-[50px] bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
    <div class="flex space-x-10">
        <div class="w-[1/3] shadow-black shadow-2xl relative rounded-[10px]">
            <img :src="photography" class="h-full rounded-[10px]">
            <RouterLink to="/photography" class="absolute top-[40%] left-[30%] transform-[-50%] text-white text-3xl bg-[rgba(0,0,0,0.6)] p-10 rounded-2xl">Photography</RouterLink>
        </div>
        <div class="w-[1/3] relative shadow-black shadow-2xl rounded-[10px] self-center">
            <img :src="paintings" class="rounded-[10px] h-full">
            <RouterLink to="/paintings" class="absolute top-[40%] left-[35%] text-white text-3xl bg-[rgba(0,0,0,0.6)] p-10 rounded-2xl">Paintings</RouterLink>
        </div>
        <div class="w-[1/3] relative shadow-black shadow-2xl rounded-[10px] self-center">
            <img :src="sculptures" class="rounded-[10px]">
            <RouterLink to="/sculptures" class="absolute top-[40%] left-[35%] text-white text-3xl bg-[rgba(0,0,0,0.6)] p-10 rounded-2xl">Sculptures</RouterLink>
        </div>
    </div>
</section>

</template>

<script setup>

import photography from '../assets/images/photography.jpg'
import paintings from '../assets/images/paintings.jpg'
import sculptures from '../assets/images/sculpture.jpg'


</script>