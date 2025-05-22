<template>

<section class="px-5 curator_pick py-[20px] md:py-[50px] bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
    <div class="container">
     <div class="countdown_header">
            <h2 class="text-center text-5xl md:text-6xl animate-pulse py-5 md:py-10 px-5">Curator's Pick Of The Day</h2>
        </div>
<div class="flex">
    <div class="grid grid-cols-1 md:grid-cols-2 md:gap-x-30">
        <div class="w-fit">
    <Countdown></Countdown>
    </div>
    <div class="relative">
 <img :src="explore_1" class="w-full">
     <div class="item bg-[#dbd0a7e3] opacity-98 py-3 px-5 text-center absolute bottom-[5%] -translate-y-[5%] left-[58%] -translate-x-[58%]">
            <h3 class="font-sig text-[18px] md:text-2xl font-semibold text-gray-500">Lola</h3>
            <h3 class="font-sig text-[16px] md:text-xl font-semibold text-gray-500">By Arifur Rahman</h3>
            <h3 class="font-sig text-[16px] md:text-xl font-semibold text-gray-500">$120</h3>
    </div>
    </div>
    </div>
</div>
    </div>
</section>

</template>

<script setup>

import explore_1 from '../assets/images/newarrival_8.jpg'
import Countdown from './Countdown.vue';

</script>