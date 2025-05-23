<template>
    <section class="banner bg-center bg-cover bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
       <div class="flex">
 <video class="w-full h-auto object-cover relative flex mx-auto" autoplay loop muted src="../assets//videos/artpiece-small.mp4" typeof="video/mp4">     
</video>
<div class="flex justify-between items-center">
 <div class="banner_text w-[50%] font-sig  text-white absolute top-[25%] left-[5%]">
        <h1 class="text-xl font-semibold md:text-6xl text-white font-sig">Welcome to Dooburi!</h1>
        <p class="w-[200px] md:w-[400px] pt-5 font-sig">We are a marketplace for curating the best art pieces in Bangladesh. Explore art pieces from a plethora of photographs, paintings and sculptures by renowned artists.
        </p>
      <RouterLink to="/paintings"><button type="submit" class="font-sig font-semibold bg-[rgba(0,0,0,0.6)] p-10 text-[20px] mx-au
         text-white shadow-2xl rounded-2xl px-10 py-3 mt-10 cursor-pointer">Explore Art Pieces</button></RouterLink>
</div>
        <div class="banner_artist absolute top-[25%] right-[10%] text-center pt-4">
        <div class="quote">
        <h1 class="font-sig text-6xl text-white text-center w-[600px]"><i class="fa-solid fa-quote-left"></i> Reality leaves a lot to the imagination. <i class="fa-solid fa-quote-right"></i> <br></h1> 
<span class="text-[50px] text-white font-sig text-center flex justify-center">- John Lennon</span>
<div>
</div>
</div>
    <h2 class="font-sig font-semibold mt-8 text-[30px] text-white">Are You An Artist?</h2>
    <h3 class="font-sig text-[16px] font-semibold text-white">Join Dooburi to exhibit your exclusive art pieces to passionate art collectors.</h3>
   <RouterLink to="/login"><button type="submit" class="font-sig font-semibold bg-[rgba(0,0,0,0.6)] p-10 text-[20px] mx-au
   text-white shadow-2xl rounded-2xl px-10 py-3 mt-5 cursor-pointer">Exhibit Your Artwork</button></RouterLink>
        <div class="container mx-auto w-[50%]"> 
    <div class="absolute top-[20%]">

</div>
</div>
</div>
</div>   
</div>

</section>
</template>
<script setup>


</script>