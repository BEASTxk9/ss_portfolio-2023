<template>
  <Suspense @pending="pending" @fallback="fallback" @resolve="resolved">

<template #default>
  <Header></Header>
</template>

<template #fallback>
  <section id="loading_sec" class="fixed-top">
<Loader></Loader>
  </section>
</template>

</Suspense>


</template>

<script setup>
// import components
import Header from '@/components/Header.vue';
import Loader from '@/components/Loader.vue';
</script>

<script>
export default{

}
</script>

<style scoped>
#loading_sec{
  padding-top: 28vh;
  background-color: white;
  max-height: 100vh;
  overflow: hidden !important;
  z-index: 50;
  transition: all 0.3s ease-in-out;
}

main{
  z-index: 2;
  background-color: white;
}

</style>