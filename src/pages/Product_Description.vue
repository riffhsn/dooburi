<template>
<section class="prod_desc py-[50px]">
    <div class="container">
        <div class="flex space-x-10">
            <div class="w-[70%]">
                <img :src="photo_1" class="w-full">
                <h2 class="font-sig text-[30px] font-semibold py-3">Enigma</h2>
                <p>Capture the serenity of nature with Whispers of Dawn, a breathtaking landscape photograph that freezes the quiet beauty of the early morning. This high-resolution image features golden light spilling over misty hills, with soft hues blending sky and earth in perfect harmony. Ideal for home or office decor, this print brings a sense of calm and connection to the natural world.
Printed on premium archival paper with rich, true-to-life colors and museum-grade longevity, each piece is signed and available in multiple sizes. Whether displayed as a statement centerpiece or part of a curated gallery wall, Whispers of Dawn adds depth, elegance, and timeless beauty to any space.</p>
                    <h3 class="font-sig text-[18px] font-semibold py-5">Keywords</h3>
                    <div class="flex items-center space-x-3">
                        <div v-for="keyword in 4" class="flex items-center px-5 space-x-3 outline-1 rounded-[4px] hover:bg-[#dbd0a7e3] hover:text-[rgba(0,0,0,0.5)]" >
                        <i class="fa-solid fa-wand-magic-sparkles"></i>
                        <p>Photos</p>
                    </div>
                        </div>
            </div>
                <div class="w-[30%]">
                <h2 class="font-sig text-[30px] font-semibold">Enigma</h2>
                <div class="flex space-x-3 py-2">
                    <p class="flex space-x-1">
                  <i v-for="star in 5" class="fa-solid fa-star text-amber-400"></i>
                    </p>
                    <p class="text-[12px] text-[rgba(0,0,0,0.5)] font-sig font-semibold">(120 Reviews)</p>
                </div>
                <div>
                    <h3 class="font-sig text-[20px] text-black py-3">$192.00</h3>
                    <p class="font-sig text-[14px] border-b-1 pb-3 border-[rgba(0,0,0,0.5)]">Capture the serenity of nature with Whispers of Dawn, a breathtaking landscape photograph that freezes the quiet beauty of the early morning. This high-resolution image features golden light spilling over misty hills, with soft hues blending sky and earth in perfect harmony. Ideal for home or office decor, this print brings a sense of calm and connection to the natural world.</p>
                </div>
                <div class="colors flex py-10 items-center space-x-5">
                    <button type="button" class="font-sig text-gray-500 font-semibold px-10 py-3 bg-[#dbd0a7e3] rounded-[4px]">Add to Cart</button>
                    <i class="fa-solid fa-heart  px-3 hover:text-red-400 shadow-2xl border-2 py-3 rounded-[4px]"></i>
                </div>
            </div>
            </div>
        </div>
</section>
</template>

<script setup>

import photo_1 from '@/assets/images/photographs_1.jpg'

import { ref } from 'vue';

const keywords = ref( [
    'photos',
    'landscape photography',
])

</script>