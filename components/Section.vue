
<script setup>

let props = defineProps(['title', 'description', 'link'])
</script>

<template>
  <section class="section">

  </section>
</template>

<style scoped>
.section{
     background-image: url("/assets/image/banner.png");
    /* height: 600px; */
    /* box-shadow: inset 0 0 0 1000px rgba(0, 0, 0, 0.8); */
    min-height: 600px;
    max-width: 100%;
    background-size: cover;
    background-repeat: no-repeat;
}
</style>