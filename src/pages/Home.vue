<template>

<Banner></Banner>
<Categories></Categories>
<About></About>
<FeaturedCollections></FeaturedCollections>
<FeaturedArtists></FeaturedArtists>
<Countdown_section></Countdown_section>
<Videos></Videos>
<News></News>
<Blog></Blog>

<section class="testimonial pb-20 pt-10 bg-cover bg-center bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
<div class="container">
    <div class="testimonial_heading">
        <h2 class="text-4xl font-bold text-center pb-10">Here's what our members are saying about us!</h2>
    </div>
    <div class="grid grid-cols-2 gap-x-10">
        <div class="testimonial_item bg-[rgba(0,0,0,0.3)] py-5 px-5 rounded-[10px] text-white">
            <div class="testimonial_text flex">
                <img :src="testimonial_1" class="w-[100px] rounded-[50%] pt-10">
            <h3 class="text-4xl pt-10">❝</h3>
            <h4 class="px-5 text-justify pt-15">I am a passionate art lover and I have purchased a few paintings from Dooburi.
                Their art pieces are of top-notch quality and delivery is prompt. I would highly recommend 
                Dooburi as your your one-stop art piece collection store!
            </h4>
            <h3 class="text-4xl pt-[150px]">❞</h3>
            </div>
            <div class="rating flex justify-start pt-10 ml-[140px]">
                <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            </div>

        </div>
        <div class="testimonial_item  bg-[rgba(0,0,0,0.3)] py-5 px-5 rounded-[10px] text-white">
            <div class="testimonial_text flex">
                <img :src="testimonial_2" class="w-[100px] rounded-[50%] pt-10">
            <h3 class="text-4xl pt-10">❝</h3>
            <h4 class="px-5 text-justify pt-15">I am a passionate art lover and I have purchased a few paintings from Dooburi.
                Their art pieces are of top-notch quality and delivery is prompt. I would highly recommend 
                Dooburi as your your one-stop art piece collection store!
            </h4>
            <h3 class="text-4xl pt-[150px]">❞</h3>
            </div>
            <div class="rating flex justify-start pt-10 ml-[140px]">
                <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star text-amber-400"></i>
            <i class="fa-solid fa-star-half text-amber-400"></i>            </div>

        </div>
      
    </div>
</div>
</section>

<Newsletter></Newsletter>


</template>

<script setup>

import Banner from '@/components/Banner.vue';
import Categories from '@/components/Categories.vue';
import About from '@/components/About.vue';
import FeaturedCollections from '@/components/FeaturedCollections.vue';
import testimonial_1 from '@/assets/images/testimonial_1.jpg'
import testimonial_2 from '@/assets/images/testimonial_2.jpg'
import Blog from '@/components/Blog.vue';
import Countdown from '@/components/Countdown.vue';
import Countdown_section from '@/components/Countdown_section.vue';
import Newsletter from '@/components/Newsletter.vue'
import News from '@/components/News.vue';
import FeaturedArtists from '@/components/FeaturedArtists.vue';
import Videos from '@/components/Videos.vue';

</script>