<template>
    <section class="py-[20px] md:py-[50px] bg-[url('https://images.pexels.com/photos/9809060/pexels-photo-9809060.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')]">
        <div class="artist_header">
            <h2 class="text-center text-5xl md:text-6xl animate-pulse py-10">Featured Artists</h2>
        </div>
  <div class="w-fit mx-auto px-4 relative">
    <div class="flex flex-col md:flex-row items-center border border-gray-500 rounded-lg shadow-xl py-10 bg-[#dbd0a7e3] opacity-95 overflow-hidden">
      <!-- Image Section -->
      <div class="w-[500px] md:w-2/3 h-64 md:h-auto">
        <img :src="slides[currentIndex].image" alt="Slide Image" class="w-full h-full object-cover" />
      </div>
      <!-- Text Section -->
      <div class="w-full md:w-1/3 p-6">
        <h2 class="text-2xl font-sig font-bold mb-2">{{ slides[currentIndex].title }}</h2>
        <h2 class="text-xl font-sig font-bold mb-2">{{ slides[currentIndex].profession }}</h2>
        <p class="text-gray-600 font-sig">{{ slides[currentIndex].description }}</p>
        <RouterLink><button type=""></button></RouterLink>

        <!-- Navigation Buttons -->
        <div class="flex space-x-2">
          <button @click="prevSlide" class="bg-gray-200 hover:bg-[#dbd0a7e3] rounded-full p-2 absolute left-0 top-[50%]">
            <span class="text-[20px] ">&larr;</span>
          </button>
          <button @click="nextSlide" class="bg-gray-200 hover:bg-[#dbd0a7e3] rounded-full p-2 absolute right-0 top-[50%]">
            <span>&rarr;</span>
          </button>
        </div>
      </div>
    </div>
  </div>
      </section>

</template>

<script setup>
import { ref } from 'vue'

const slides = ref([
  {
    image: 'https://images.pexels.com/photos/1043331/pexels-photo-1043331.jpeg?auto=compress&cs=tinysrgb&w=600',
    title: 'Patrick Garcia',
    profession: 'Painter',
    description: 'Patrick is a painter with 10 years of experience in the creative field. He has produced some great art pieces to display his expertise. ',
  },
  {
    image: 'https://images.pexels.com/photos/6714316/pexels-photo-6714316.jpeg?auto=compress&cs=tinysrgb&w=600&h=750&dpr=1',
    title: 'Adam Troy',
    profession: 'Sculptor',
    description: 'Adam is a sculptor with 10 years of experience in the creative field. He has produced some great art pieces to display his expertise.',
  },
  {
    image: 'https://images.pexels.com/photos/1264210/pexels-photo-1264210.jpeg?auto=compress&cs=tinysrgb&w=600&h=750&dpr=1',
    title: 'Anna Wintour',
    profession: 'Photographer',
    description: 'Anna is a photographer with 10 years of experience in the creative field. He has produced some great art pieces to display his expertise.',
  },
])

const currentIndex = ref(0)

function prevSlide() {
  currentIndex.value = (currentIndex.value - 1 + slides.value.length) % slides.value.length
}

function nextSlide() {
  currentIndex.value = (currentIndex.value + 1) % slides.value.length
}
</script>

<style scoped>
/* Optional custom styling */
</style>
