<template>

<section class="signup bg-center bg-cover py-[100px] bg-[url('https://images.pexels.com/photos/375882/pexels-photo-375882.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
<div class="container">
    <div class="flex justify-center">
        <form method="" action="" class="w-[600px] bg-white py-[100px] opacity-90 shadow-4xl drop-shadow-white rounded-2xl">
        <div class="signup_header text-center">
        <h2 class="font-sig font-semibold text-3xl">Join Dooburi!</h2>
        <p class="font-sig text-[14px] text-gray-400">Already joined? <a href="" class="font-sig text-[14px] text-blue-400">Sign in now</a></p>
    </div>
    <div class="px-[50px]">
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Your Name</label>
        <input type="text" placeholder="Enter Your Full Name" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <div class="px-[50px]">
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Your Email</label>
        <input type="text" placeholder="Enter Your Email" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <div class="px-[50px]">
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Password</label>
        <input type="password" placeholder="Enter Your Password" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
        <p class="font-sig text-[14px] pt-1 text-red-400">* Your password must be at least 8 characters long and include a number, an uppercase letter and a lowercase letter </p>
    </div>
    <div class="px-[50px]">
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Confirm Password</label>
        <input type="password" placeholder="Confirm Your Password" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <button type="submit" class="font-sig text-white font-semibold text-[16px] mt-10 flex mx-auto py-3 px-30 bg-[#6ca85e] rounded-2xl">Sign Up</button>
    </form>
    </div>
</div>


</section>



</template>

<script setup>



</script>