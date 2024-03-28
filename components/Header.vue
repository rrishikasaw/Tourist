<script setup></script>

<template>
  <nav>
    <v-sheet height="70" elevation="4" class="d-flex align-center nav-color">
      <v-row>
        <v-col>
          <NuxtLink to="/" class="text-white text-decoration-none ps-4"
            >Logo</NuxtLink
          >
        </v-col>
        <v-col cols="auto">
          <NuxtLink to="/" class="text-white text-decoration-none text ps-2"
            >Home</NuxtLink
          >
          <NuxtLink
            to="/about"
            class="text-white text-decoration-none text ps-4"
            >About</NuxtLink
          >
          <NuxtLink
            to="/package"
            class="text-white text-decoration-none text ps-4"
            >Package</NuxtLink
          >

          <NuxtLink
            to="/contact"
            class="text-white text-decoration-none text ps-4"
            >Contact</NuxtLink
          >

           <NuxtLink
            to="/tours"
            class="text-white text-decoration-none text ps-4"
            >Tours and Travels</NuxtLink
          >
        </v-col>
      </v-row>
    </v-sheet>
    <div class="mb-20"></div>
  </nav>
</template>

<style scoped>
a {
  font-size: 30px;
}

.nav-color {
  background: #216f8c;
  top: 0;
  position: fixed;
  width: 100%;
  z-index: 5;
}

.mb-20 {
  margin-bottom: 80px;
}
.text {
  font-size: 18px;
  margin-right: 12px;
}
</style>
