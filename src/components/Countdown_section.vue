<template>

<section class="bg-cover bg-center bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
    <div class="countdown_header py-5">
            <h2 class="text-center text-6xl animate-pulse py-10">Curator's Pick Of The Day</h2>
        </div>
<div class="flex items-cen">
    <div class="w-1/2 flex justify">
    <Countdown></Countdown>
</div>
<div class="w-1/2">
    <div class="relative mr-[100px] py-[250px] bg-cover bg-center bg-[url('https://images.pexels.com/photos/1707640/pexels-photo-1707640.jpeg?auto=compress&cs=tinysrgb&w=600')]"></div>
    <div class="item text-center py-3">
            <h3 class="font-sig text-2xl font-semibold text-[rgba(0,0,0,0.9)]">Lola</h3>
            <h3 class="font-sig text-xl font-semibold text-[rgba(0,0,0,0.9)]">By Arifur Rahman</h3>
            <h3 class="font-sig text-xl font-semibold text-[rgba(0,0,0,0.9)]">$120</h3>
    </div></div>
</div>
</section>

</template>

<script setup>

import Countdown from './Countdown.vue';

import explore_1 from '../assets/images/artist_2.jpg'

</script>