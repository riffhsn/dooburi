<template>

<section class="checkout py-[50px]">

<div class="container">
    <div class="flex gap-x-20">
        <div class="w-[50%]">
            <div class="checkout_head">
    <h2 class="font-sig font-semibold text-3xl">Billing Details</h2>
</div>
<form method="POST" action="">
    <div>
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Full Name<span class="text-red-400">*</span></label>
        <input type="text" placeholder="Enter Your Full Name" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <div>
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Company Name</label>
        <input type="text" placeholder="Enter Your Company Name" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <div>
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Street Address<span class="text-red-400">*</span></label>
        <input type="text" placeholder="Enter Your Street Details" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <div>
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Apartment, floor, etc.</label>
        <input type="text" placeholder="Enter Your Address Details" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
    </div>
    <div>
        <label class="font-sig text-[14px] text-black font-semibold block py-3">Town/City</label>
        <select>
            <option>Dhaka</option>
            <option>Chittagong</option>
            <option>Sylhet</option>
            <option>Rajshahi</option>
            <option>Khulna</option>
            </select>
            <div>
                <label class="font-sig text-[14px] text-black font-semibold block py-3">Phone Number<span class="text-red-400">*</span></label>
                <input type="text" placeholder="Enter Your Phone Number" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
        </div>
        <div>
                <label class="font-sig text-[14px] text-black font-semibold block py-3">Email Address<span class="text-red-400">*</span></label>
                <input type="email" placeholder="Enter Your Email Address" class="font-sig text-[14px] block py-3 px-5 border-1 border-[rgba(0,0,0,0.3)] w-full rounded-2xl">
        </div>
        </div>
</form>
        </div>
        <div class="w-[50%] py-20">
<div>
    <div class="order flex py-3 items-center" v-for="cart in carts">
        <div class="flex items-center">
        <img :src="cart.image" class="w-[15%]">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5">{{ cart.name }}</h3>
        </div>
        <div><h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5">${{ cart.price }}</h3></div>
    </div>
    <div class="border-b-1 border-gray-400">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Subtotal:</h3>
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5"></h3>
    </div>
    <div class="border-b-1 border-gray-400 flex items-center justify-between">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Shipping:</h3>
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5">Free</h3>
    </div>
    <div class="flex items-center">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Total:</h3>
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5 flex justify-end"></h3>
    </div>
    <button type="button" class="font-sig text-gray-500 font-semibold px-10 py-3 bg-[#dbd0a7e3] rounded-[4px] mt-10">Place Order</button>
</div>
</div>
    </div>
</div>

</section>

</template>

<script setup>

import { ref } from 'vue';

const carts = ref([
    {
    id: '1',
    image: 'https://images.pexels.com/photos/147411/italy-mountains-dawn-daybreak-147411.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
    name: 'Scenic Heaven',
    artist: 'Adam Jose',
    quantity: '1',
    price: '120'
},

{
    id: '2',
    image: 'https://images.pexels.com/photos/1269968/pexels-photo-1269968.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
    name: 'Enigma',
    artist: 'Rose Emilia',
    price: '320'
},

{
    id: '3',
    image: 'https://images.pexels.com/photos/922610/pexels-photo-922610.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1', 
    name: 'Melody',
    artist: 'Allen James',
    price: '220'
}
])



</script>