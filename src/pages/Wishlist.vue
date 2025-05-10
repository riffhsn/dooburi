<template>

<section class="wishlist py-20">
<div class="container">
<h2 class="font-sig text-[20px] leading-6 pb-[60px]">Wishlist (4)</h2>
<div class="flex space-x-[30px]">
    <div v-for="product in 4" :key="product" class="w-1/4">
<div>
<div class="wishlist_items pt-[45px] pb-[80px] px-[40px] bg-[#e8ddc5] rounded-[10px] relative">
<img :src="wishlist" class="mx-auto">
<RouterLink><i class="fa-solid fa-trash absolute right-0 bottom-[20px] p-2 bg-white rounded-[50%] mt-[12px] mr-[12px]" ></i></RouterLink>
</div>
<div>
    <h4 class="text-[16px] leading-6 font-popo font-medium text-black pt-4">Westershire</h4>
    <p><span class="text-gray-500 text-[16px] font-sig leading-6 pr-3 font-semibold">$960</span></p>
</div>
</div>
</div>
</div>
</div>
</section>
</template>
<script setup>

import wishlist from '@/assets/images/paintings_1.jpg'

</script>