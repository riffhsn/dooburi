<template>

<section class="blog py-[20px] md:py-[50px] px-[50px] bg-center bg-cover bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
    <h2 class="text-center text-5xl md:text-6xl animate-pulse py-10">Blogs</h2>
            <div class="flex gap-x-10">
        <div v-for="blog in blogs" :key="blog" class="relative">
            <div >
                <img :src="blog.image" class="w-fit">
            </div>
            <div class="blog_text w-fit absolute top-[50%] -translate-y-[50%] left-[50%] -translate-x-[50%] text-center px-5 py-10 bg-[rgba(0,0,0,0.3)]">
        <h3 class="font-sig text-[16px] font-semibold text-white">{{blog.title}}</h3>
        <h3 class="font-sig text-[14px] font-normal text-white">By {{ blog.contributor }}</h3>
        <a href="" class="text-white font-sig text-[14px]">Read More..</a> 
        <h3 class="font-sig text-white text-[12px] mt-4">Published:{{ blog_date }}</h3>
            </div>
    </div>
    </div>
   </section>
</template>

<script setup>
import { ref } from 'vue';

const blogs = ref([{
    id: '1',
    image: 'https://images.pexels.com/photos/1981468/pexels-photo-1981468.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
    title:'How to preserve artwork',
    contributor: 'Arthur Conan',
    description: '',
},

{
    id: '2',
    image: 'https://images.pexels.com/photos/933255/pexels-photo-933255.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
    title:'Am I Even Cut Out to Be an Artist?',
    contributor: 'John Doe',
    description: 'This week, we’re responding to an artist who’s been making art for years—but finds themselves exhausted by the pressure to turn it into a business. They’re wondering if they’re even cut out for this, struggling with burnout, pricing, and questioning whether their work still matters in a world that feels increasingly disconnected from the value of human-made art. ',
},

{
    id: '3',
    image: 'https://images.pexels.com/photos/7655645/pexels-photo-7655645.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
    title:'This Artist uses waste to produce art pieces',
    contributor: 'Paul Taylor',
    description: 'This week, we’re responding to an artist who’s been making art for years—but finds themselves exhausted by the pressure to turn it into a business. They’re wondering if they’re even cut out for this, struggling with burnout, pricing, and questioning whether their work still matters in a world that feels increasingly disconnected from the value of human-made art. ',
}, 

{
    id: '4',
    image: 'https://images.pexels.com/photos/1264210/pexels-photo-1264210.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1',
    title:'Learn basics of Photography',
    contributor: 'Emily Rue',
    description: 'This week, we’re responding to an artist who’s been making art for years—but finds themselves exhausted by the pressure to turn it into a business. They’re wondering if they’re even cut out for this, struggling with burnout, pricing, and questioning whether their work still matters in a world that feels increasingly disconnected from the value of human-made art. ',
}])

const blog_date = new Date();

</script>