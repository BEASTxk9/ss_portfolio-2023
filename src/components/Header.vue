<template>
    <header id="landingpage_bg" class="fixed-top"> 
    </header>
<section>
<h1>header</h1>
</section>
</template>

<script setup>
// import package for Loader function
import { ref } from 'vue';

// Loader function
const data = ref(null);
const getData = async () => {
await new Promise((resolve) => setTimeout(resolve, 5000));
data.value = {
  main_header : 'Header',
  sub_header : 'Sub Header'
}
};
await getData();
</script>

<style scoped>
#landingpage_bg{
    background-image: url('https://i.postimg.cc/prK51QGk/pexels-pixabay-355770.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    z-index: -1;
    min-height: 100vh;
  }
</style>