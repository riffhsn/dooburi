<template>
 
<section class="">
<div class="flex">
    <div class="w-1/2 py-[150px] px-20 bg-cover bg-center bg-[url('https://images.pexels.com/photos/13312438/pexels-photo-13312438.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
        <h2 class="font-sig font-semibold text-3xl text-white">Welcome To Our Community!</h2>
        <p class="font-sig text-white font-semibold py-3 pr-20 text-justify">Welcome to Dooburi! The hub for art enthusiasts and artists. Join our community and enter the world of art. This is a digital platform where artists exhibit their art pieces and art enthusiasts can collect their favorite artworks. Engage with our community and stay connected to your inner artist. </p>
    </div>
    <div class="w-1/2 py-[100px] px-[100px]">
        <h2 class="font-sig font-semibold text-3xl text-black py-5">Welcome Back!</h2>
        <p class="font-sig font-semibold text-[16px] text-gray-500 py-5 pr-[300px]">Welcome back to Dooburi's world of creative art pieces. Login to explore curated art pieces from Dooburi.</p>
       <form action="" method="">
        <div class="w-1/2">
                <label class="font-sig text-[14px] text-black font-semibold block py-3">Email Address<span class="text-red-400">*</span></label>
                <input type="email" placeholder="Enter Your Email Address" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
        </div>
        <div class="w-1/2">
                <label class="font-sig text-[14px] text-black font-semibold block py-3">Password<span class="text-red-400">*</span></label>
                <input type="password" placeholder="Enter Your Password" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
        </div>
        <div class="flex space-x-10">
            <div class="flex space-x-3">
            <input type="checkbox">
            <label class="font-sig text-[14px] text-black font block py-3">Remember me</label>
        </div>
        <div class="flex space-x-3">
            <input type="checkbox">
            <label class="font-sig text-[14px] text-black font block py-3">Forgot Password</label>
        </div>
        </div>
        <div>
            <button type="submit" class="bg-[#dbd0a7e3] font-sig text-[16px] font-semibold text-gray-500 cursor-pointer rounded-[4px] py-4 px-12 mt-4">Login</button>
            <p class="font-sig font-semibold text-[12px] text-gray-500 py-5 pr-[300px]"> Don't have an account? <RouterLink to="/user" class="font-sig font-semibold text-[12px] text-blue-400 py-5">Create a free account</RouterLink> </p>
        </div>
    </form>
    </div>
</div>
</section>
</template>

<script setup>

</script>