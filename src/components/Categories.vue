<template>
<section class="categories py-[120px] px-[50px] bg-center bg-cover bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
            <div class="grid grid-cols-4 space-y-10
             gap-x-10 justify-center">
            <div class="w-fit" v-for="category in categories" :key="category" >
        <div class="shadow-black shadow-2xl relative rounded-[10px]">
            <img :src="category.image" class="rounded-[10px]  w-[400px] h-[300px]">
            <RouterLink to="/photography" class="absolute top-[40%] left-[30%] text-white text-2xl bg-[rgba(0,0,0,0.6)] py-3 px-5 rounded-2xl">{{category.name}}</RouterLink>
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
        image: 'https://images.pexels.com/photos/792381/pexels-photo-792381.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
        name: 'Photography',
    },
    
    {
        id: '2',
        image: 'https://images.pexels.com/photos/102127/pexels-photo-102127.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
        name: 'Paintings',
    },
    
    {
        id: '3',
        image: 'https://images.pexels.com/photos/5393589/pexels-photo-5393589.jpeg?auto=compress&cs=tinysrgb&w=600', 
        name: 'Sculptures',
    },
    {
        id: '4',
        image: 'https://images.pexels.com/photos/4238489/pexels-photo-4238489.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
        name: 'Digital Art',
    }, 
    {
        id: '5',
        image: 'https://images.pexels.com/photos/2838545/pexels-photo-2838545.jpeg?auto=compress&cs=tinysrgb&w=600', 
        name: 'Illustrations',
    },
    
    {
        id: '6',
        image: 'https://images.pexels.com/photos/357428/pexels-photo-357428.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
        name: 'Pottery',
    },
    
    {
        id: '7',
        image: 'https://www.singulart.com/blog/wp-content/uploads/2020/07/marilyn.jpg', 
        name: 'Pop Art',
    },
    {
        id: '8',
        image: 'https://www.seedandspark.com.au/uploads/1/0/2/7/102754722/s254093505207171772_p406_i15_w4696.jpeg?width=640', 
        name: 'Resin Art',
    },
    ])
    


</script>