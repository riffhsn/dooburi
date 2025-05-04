<template>

<Nav></Nav>
<RouterView></RouterView>
<Footer></Footer>

</template>

<script setup>

import Nav from './components/Nav.vue';
import { RouterView } from 'vue-router';
import Footer from './components/Footer.vue';

</script>