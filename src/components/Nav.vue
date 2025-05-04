<template>

<section class="navbar py-5 bg-[#e8ddc5] font-sig">
    <div class="container">
        <div class="flex justify-between items-center">
        <div class="menu w-[3/5] flex justify-start space-x-5">
            <ul v-for="menu in menubar">
                <li class="text-gray-500 text-[16px] leading-4 py-4 font-semibold font-sig"><RouterLink>{{menu}}</RouterLink></li>
            </ul>
            <div>
        <form action="" method="">
        <input class="bg-gray-200 px-5 py-2 w-[300px] focus:outline-none rounded-2xl text-black" placeholder="What are you looking for?">
    </form>
    </div>
</div>
<div class="logo w-[1/5]">
  
</div>
<div class="flex justify-end">
<div class="w-[1/5] px-5">
    <div class="icons flex justify-end space-x-5 items-center">
    <RouterLink to="/cart"><i class="fa-solid fa-bag-shopping text-gray-500"></i></RouterLink> 
    <RouterLink><i class="fa-solid fa-user text-[18px] text-gray-500"></i></RouterLink>
   <RouterLink> <i class="fa-solid fa-heart text-gray-500 text-[18px]"></i> </RouterLink>
   <RouterLink to="/signup"><button type="button" class="font-sig font-semibold bg-[rgba(0,0,0,0.3)] px-3 py-2 rounded-2xl text-[16px] text-white"> Signup </button></RouterLink> 
   <RouterLink to="/login"><button type="button" class="font-sig font-semibold bg-[rgba(0,0,0,0.3)] px-3 py-2 rounded-2xl text-[16px] text-white"> Login </button></RouterLink> 

</div>
    </div>
</div>
    </div>
    </div>

</section>
</template>

<script setup>

import { ref } from 'vue';

const menubar = ref(
    [
    'Home',
    'Explore Artpieces',
    'Login'
    ]
)

</script>