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
    <div class="flex justify-between border-b-1 border-gray-400">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Subtotal:</h3>
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5">${{subtotal}}</h3>
    </div>
    <div class="border-b-1 border-gray-400 flex items-center justify-between">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Shipping:</h3>
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5">Free</h3>

    </div>
    <div class="flex items-center justify-between">
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Total:</h3>
        <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3 px-5 flex justify-end">${{ subtotal }}</h3>
    </div>
            <div>
            <h3 class="font-sig font-semibold text-[16px] text-gray-500  py-3">Payment Option</h3>
            <div class="flex items-center space-x-2">
          <input type="radio" id="payment1" name="payment_method">
          <label class="font-sig text-[14px] text-black font-semibold block py-3" for="payment1">Cash On Delivery</label>
            </div>
            <div class="flex items-center space-x-2">
        <input type="radio" id="payment2" name="payment_method">
          <label class="font-sig text-[14px] text-black font-semibold block py-3" for="payment2">Debit/Credit Card</label>
            </div>
            <div class="flex items-center space-x-2">
        <input type="radio" id="payment3" name="payment_method">
          <label class="font-sig text-[14px] text-black font-semibold block py-3" for="payment3">Bkash</label>
            </div>
        </div>
    <button type="button" class="font-sig text-gray-500 font-semibold px-10 py-3 bg-[#dbd0a7e3] rounded-[4px] mt-10">Place Order</button>
</div>
</div>
    </div>
</div>
</section>

</template>

<script setup>

import { ref, computed } from 'vue';
    import cart1 from '../assets/images/newarrival_3.jpg'
    import cart2 from '../assets/images/newarrival_2.jpg'

    const carts = ref([
    {id: 1,
        name: 'Angel Hope',
        price: '550',
        image: cart1,
        count:1
    },
    
    {id: 2,
        name: 'Ray of Hope',
        price: '550',
        image: cart2,
        count:1
    }
    ])

const subtotal = computed(() =>
        carts.value.reduce((acc, cart) => acc + cart.price * cart.count, 0))

</script>