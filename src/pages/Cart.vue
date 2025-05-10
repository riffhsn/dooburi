<template>

    <section class="Cart pb-[110px] pt-[50px]">
    <div class="container">
        <div><h2 class="text-center text-5xl py-10">Your Cart</h2>
        </div>
        <div class="flex shadow-xl">
            <div class="w-[25%] flex shadow-custom">
                <h3 class="text-[16px] font-popo leading-6 py-6 pl-[40px]">Product</h3>
        </div>
        <div class="w-[25%] flex justify-center shadow-custom">
                <h3 class="text-[16px] font-popo leading-6 shadow-2xl py-6">Price</h3>
        </div>
        <div class="w-[25%] flex justify-center shadow-custom">
                <h3 class="text-[16px] font-popo leading-6 py-6">Quantity</h3>
                </div>
                <div class="w-[25%] flex justify-end shadow-custom">
                <h3 class="text-[16px] font-popo leading-6 py-6 pr-10">Subtotal</h3>
        </div>
        </div>
        <div v-for="(cart, index) in carts" class="flex py-8 px-10 shadow-xl mt-10">
            <div class="flex w-1/4 items-center">
                <img :src="cart.image">
                <h3 class="text-[16px] font-popo leading-6 pl-5">{{ cart.name }}</h3>
            </div>
            <div class="flex w-1/4 items-center justify-center">
                <h3 class="text-[16px] font-popo leading-6">${{ cart.price }}</h3>
            </div>
            <div class="flex w-1/4 items-center justify-center mt-10">
                <div class="flex border-[1.5px] border-[rgba(0,0,0,0.4)] rounded-[4px] px-3 py-1">
                <input type="text" :value="cart.count" class="w-full outline-0">    
                <div>
                <i @click="increment(index)" class="fa-solid fa-chevron-up w-[5px] h-[8.5px]"></i>
                <i @click="decrement(index)" class="fa-solid fa-chevron-down w-[5px] h-[8.5px]"></i>
            </div>
                </div>
            </div>
            <div class="flex w-1/4 items-center justify-end">
                <h3 class="text-[16px] font-popo leading-6 pr-[40px]">${{ cart.price * cart.count }}</h3>
            </div>
        </div>
        <div class="flex justify-between">
            <button type="submit" class="bg-[#dbd0a7e3] text-[16px] text-[rgba(0,0,0,0.5)] font-popo leading-6 font-medium px-12 py-4 rounded-[4px] mt-6">Return To Shop</button>
            <button type="submit" class="bg-[#dbd0a7e3] text-[16px] font-popo leading-6 font-medium flex px-12 py-4 text-[rgba(0,0,0,0.5)] rounded-[4px] mt-6">Update Cart</button>
        </div>
        <div class="flex justify-end">
            <div class="w-1/3 py-8 px-6 border-[1.5px] rounded-[4px] mt-[112px]">
            <h2 class="text-[20px] font-popo leading-7 font-medium pb-6">Cart Total</h2>
            <div class="flex justify-between pb-4 border-b-1 border-[rgba(0,0,0,0.4)]">
                <h3 class="font-popo text-[16px] leading-6">Subtotal:</h3>
                <h3 class="font-popo text-[16px] leading-6">${{ subtotal }}</h3>
            </div>
            <div class="flex justify-between py-2 border-b-1 border-[rgba(0,0,0,0.4)]">
                <h3 class="font-popo text-[16px] leading-6">Shipping:</h3>
                <h3 class="font-popo text-[16px] leading-6">Free</h3>
            </div>
            <div class="flex justify-between py-2 border-b-1 border-[rgba(0,0,0,0.4)]">
                <h3 class="font-popo text-[16px] leading-6">Total:</h3>
                <h3 class="font-popo text-[16px] leading-6">${{ subtotal }}</h3>
            </div>
           <RouterLink to="/checkout"><button type="submit" class="bg-[#dbd0a7e3] font-sig text-[16px] font-medium text-gray-500 cursor-pointer rounded-[4px] py-4 px-12 mt-4 flex mx-auto">Proceed to checkout</button></RouterLink> 
        </div> 
        </div>
        </div>
    </section>
    
    </template>
    
    <script setup>
       
    import {ref, computed} from 'vue';
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
    
    const increment = (index)=> {
        carts.value[index].count++
    }
    
    const decrement = (index)=> {
        if(carts.value[index].count > 1){
            carts.value[index].count--
        }
    }
    
    const subtotal = computed(() =>
        carts.value.reduce((acc, cart) => acc + cart.price * cart.count, 0))
    

    
    </script>