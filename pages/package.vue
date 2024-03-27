<script setup></script>

<template>
  <section class="section d-flex justify-center align-center">
    <div>
      <h1 class="text-center pt-10 text-white Enjoy">Packages</h1>
    </div>
  </section>
  <v-container>
    <Package />
  </v-container>
</template>
<style scoped>
.Enjoy {
  font-size: 60px;
  font-weight: bold;
  padding-top: 100px;
}
.joy {
  font-size: 19px;
}
.section {
  background-image: url('/assets/image/section/section1-banner2.jpg');
  /* height: 600px; */
  box-shadow: inset 0 0 0 1000px rgba(0, 0, 0, 0.7);
  min-height: 600px;
  max-width: 100%;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
