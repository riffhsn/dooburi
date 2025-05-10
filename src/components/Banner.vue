<template>
    <section class="banner">
        <video class="w-full relative" autoplay loop muted src="../assets//videos/artpiece.mp4" typeof="video/mp4">
        </video>
        <div class="flex absolute top-[25%] left-0">
    <div class="banner_text font-sig ml-[200px] w-[40%] text-white">
        <h1 class="text-6xl text-white font-sig">Welcome to Dooburi!</h1>
        <p class="w-[400px] pt-5 font-sig">We are a marketplace for curating the best art pieces in Bangladesh. Explore art pieces from a plethora of photographs, paintings and sculptures by renowned artists.
        </p>
        <button type="submit" class="font-sig font-semibold bg-[rgba(0,0,0,0.6)] p-10 text-[20px] mx-au
         text-white shadow-2xl rounded-2xl px-10 py-5 mt-10 cursor-pointer">Explore Art Pieces</button>
    </div>
    <div class="quote w-[60%]">
        <h1 class="font-sig text-6xl text-white text-center"><i class="fa-solid fa-quote-left"></i> Reality leaves a lot to the imagination. <i class="fa-solid fa-quote-right"></i> <br></h1> 
<span class="text-[50px] text-white font-sig text-center flex justify-center">- John Lennon</span>
<div>
</div>
<div class="relative text-center">
<img :src="artist_banner" class="w-1/2 rounded-2xl text-center mt-10 ml-[250px] opacity-95">
  <h2 class="text-[30px] text-white font-sig text-center absolute top-0 left-[38%] py-10">Are You An Artist?</h2>
  <p class="absolute top-[30%] left-[30%] font-sig text-[18px] text-white w-[380px]"> Join Dooburi to display your creativity and art works to the world. </p>
  <RouterLink to="/signup/artist"><button type="submit" class=" font-sig font-semibold bg-[rgba(0,0,0,0.6)] p-10 text-[18px] absolute top-[50%] left-[40%] flex justify-center mx-auto
         text-white shadow-2xl cursor-pointer rounded-2xl px-10 py-5">Sell Your Art</button></RouterLink>
</div>
    </div>
</div>
</section>

</template>
<script setup>

import artist_banner from '@/assets/images/painting_banner.jpg'

</script>