<template>
    <section class="banner bg-center bg-cover bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
       <div class="flex">
 <video class="h-[70%] w-[50%] relative flex mx-auto" autoplay loop muted src="../assets//videos/artpiece-small.mp4" typeof="video/mp4">
        </video>
            <div class="banner_text font-sig  w-[40%] text-white absolute top-[25%] left-[5%]">
        <h1 class="text-6xl text-white font-sig">Welcome to Dooburi!</h1>
        <p class="w-[400px] pt-5 font-sig">We are a marketplace for curating the best art pieces in Bangladesh. Explore art pieces from a plethora of photographs, paintings and sculptures by renowned artists.
        </p>
      <RouterLink to="/paintings"><button type="submit" class="font-sig font-semibold bg-[rgba(0,0,0,0.6)] p-10 text-[20px] mx-au
         text-white shadow-2xl rounded-2xl px-10 py-5 mt-10 cursor-pointer">Explore Art Pieces</button></RouterLink>
    </div>
    <div class="container mx-auto"> 
    <div class="absolute top-[20%] ">
    <div class="quote">
        <h1 class="font-sig text-6xl text-[rgba(0,0,0,0.9)] text-center"><i class="fa-solid fa-quote-left"></i> Reality leaves a lot to the imagination. <i class="fa-solid fa-quote-right"></i> <br></h1> 
<span class="text-[50px] text-[rgba(0,0,0,0.9)] font-sig text-center flex justify-center">- John Lennon</span>
<div>
</div>

</div>
<div class="banner_artist text-center pt-4">
    <h2 class="font-sig font-semibold text-[30px] text-[rgba(0,0,0,0.9)]">Are You An Artist?</h2>
    <h3 class="font-sig text-[16px] font-semibold">Join Dooburi to exhibit your exclusive art pieces to passionate art collectors.</h3>
   <RouterLink to="/login"><button type="submit" class="font-sig font-semibold bg-[rgba(0,0,0,0.6)] p-10 text-[20px] mx-au
   text-white shadow-2xl rounded-2xl px-10 py-5 mt-5 cursor-pointer">Exhibit Your Artwork</button></RouterLink>
</div>
</div>

</div>
</div>
   

</section>
</template>
<script setup>

import artist_banner from '@/assets/images/painting_banner.jpg'

</script>