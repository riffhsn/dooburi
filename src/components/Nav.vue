<template>

<section class="navbar flex items-center py-5 bg-[#e8ddc5] font-sig">
    <div class="container">
        <div class="flex justify-between items-center">
            <div class="logo w-[1/5]">
</div>
        <div class="menu absolute w-[2/5] items-center flex justify-start space-x-20">
            <ul class="flex space-x-5 font-sig font-semibold text-gray-500 text-[16px]">
              <RouterLink to="/"> <li><a>Home</a></li> </RouterLink>
                <li><a href="">Artworks</a>
                <ul class="hidden hover:visible delay-75">
                <RouterLink to="/paintings"> <li><a>Paintings</a></li> </RouterLink>
                <RouterLink to="/photography"> <li><a>Photographs</a></li> </RouterLink>
                <RouterLink to="/sculptures"><li><a>Sculptures</a></li></RouterLink>
                </ul>
                </li>
              <li><a>Artists</a></li>
             <li><a>Featured Collections</a></li>
             <li><a>Videos</a></li>
             <li> <a href="#">Blogs</a> </li>
            </ul>
            <div>
        <form action="" method="" class="flex justify-end">
        <input class="bg-gray-200 px-5 py-2 w-[300px] focus:outline-none rounded-2xl text-black" placeholder="What are you looking for?">
    </form>
    </div>
</div>
<div class="flex justify-center items-center">
<div class="w-[2/] px-5">
    <div class="icons space-x-3">
    <RouterLink to="/user"><i class="fa-solid fa-user text-[18px] text-gray-500"></i></RouterLink>
   <RouterLink to="/wishlist"> <i class="fa-solid fa-heart text-gray-500 text-[18px]"></i> </RouterLink>
   <RouterLink to="/cart" class="text-gray-500 text-[18px]"><i class="fa-solid fa-bag-shopping"></i></RouterLink>
</div>
    <div>
</div>
    <div class="icons flex space-x-5 items-center">
</div>
    </div>
</div>
    </div>
    </div>
</section>
</template>

<script setup>

</script>