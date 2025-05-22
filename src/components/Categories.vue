<template>

<section class="hidden categories py-[120px] px-[50px] bg-center bg-cover bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
            <div class="grid grid-cols-4 space-y-10 gap-x-10 justify-center">
            <div class="w-full" v-for="category in categories" :key="category" >
        <div class="shadow-black shadow-2xl relative rounded-[10px]">
            <img :src="category.image" class="rounded-[10px] h-[600px] w-full">
            <RouterLink to="/photography" class="absolute top-[50%] -translate-y-[50%] left-[50%] -translate-x-[50%] text-white text-2xl bg-[rgba(0,0,0,0.6)] py-3 px-5 rounded-2xl">{{category.name}}</RouterLink>
        </div>
    </div>
    </div>
</section>
</template>

<script setup>

 import { ref } from 'vue';
    
    const categories = ref([
        {
        id: '1',
        image: 'https://images.pexels.com/photos/1447264/pexels-photo-1447264.jpeg?auto=compress&cs=tinysrgb&w=600', 
        name: 'Photography',
    },
    
    {
        id: '2',
        image: 'https://images.pexels.com/photos/2372978/pexels-photo-2372978.jpeg?auto=compress&cs=tinysrgb&w=600', 
        name: 'Paintings',
    },
    
    {
        id: '3',
        image: 'https://images.pexels.com/photos/6714806/pexels-photo-6714806.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
        name: 'Sculptures',
    },
        {
        id: '4',
        image: 'https://images.pexels.com/photos/29889876/pexels-photo-29889876/free-photo-of-cozy-indoor-knitting-session-with-tea.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
        name: 'Crafts',
    },
    ])

</script>

