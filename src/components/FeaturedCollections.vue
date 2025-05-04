<template>
    <section class="blog py-[100px] px-[50px] bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
       <div class="featured_collectionhead">
        <h2 class="text-center text-6xl animate-pulse py-10">Featured Collections</h2>
       </div>
       <div class="flex items-center">
                <div class="w-[1/3] flex justify-center">
            <div class=" space-y-10">
                <div class="relative text-center flex justify-center">
                    <img :src="featuredcoll_1" class="w-[75%] ">
                    <h3 class="absolute top-[40%] left-[32%] font-sig text-white font-semibold text-[25px] flex justify-center py-3 px-10 bg-[rgba(0,0,0,0.5)] rounded-2xl">Animal Photography</h3>
                   <RouterLink to="/animal_photography" class="absolute top-[50%] left-[40%] font-sig text-white font-semibold text-[16px] text-center flex mx-auto py-3 px-10 bg-[rgba(0,0,0,0.5)] rounded-2xl"> View Collection </RouterLink>
                </div>
                <div>
                </div>
        </div>
        </div>
        <div class="w-[1/3] mx-auto space-y-10">
            <div>
                <div class="relative justify-center flex">
                    <img :src="abstract_bg" class="w-full">
                    <h3 class="absolute top-[40%] left-[32%] font-sig text-white font-semibold text-[25px] flex justify-center py-3 px-10 bg-[rgba(0,0,0,0.5)] rounded-2xl">Abstract Paintings</h3>
                   <RouterLink to="/abstract_paintings" class="absolute top-[50%] left-[38%] font-sig text-white font-semibold text-[16px] text-center flex mx-auto py-3 px-10 bg-[rgba(0,0,0,0.5)] rounded-2xl mt-10"> View Collection </RouterLink>

                </div>
        </div>
        <div>
                <div class="relative justify-center flex">
                    <img :src="sculpture_1" class="w-[50%]">
                    <h3 class="absolute top-[40%] left-[37%] font-sig text-white font-semibold text-[25px] flex justify-center py-3 px-10 bg-[rgba(0,0,0,0.5)] rounded-2xl">Sculptures</h3>
                   <RouterLink to="/sculptures" class="absolute top-[50%] left-[38%] font-sig text-white font-semibold text-[16px] text-center flex mx-auto py-3 px-10 bg-[rgba(0,0,0,0.5)] rounded-2xl mt-5"> View Collection </RouterLink>
                </div>
        </div>
        </div>

       </div>
       </section>
    </template>
    
    <script setup>
    
    import featuredcoll_1 from '@/assets/images/photography.jpg'
    import abstract_bg from '../assets/images/abstract_bg.jpg'
    import sculpture_1 from '../assets/images/sculpture.jpg'
    
    </script>