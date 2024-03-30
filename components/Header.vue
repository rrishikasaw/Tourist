<script setup></script>

<template>
  <nav>
    <v-sheet height="70" elevation="4" class="d-flex align-center nav-color">
      <v-row>
        <v-col>
          <NuxtLink to="/" class="text-white text-decoration-none ps-4"
            >
            <img src="../assets/image/logo/logo.jpg" alt="" width="70">
            
            </NuxtLink
          >
        </v-col>
        <v-col cols="auto">
          <NuxtLink to="/" class="text-white text-decoration-none text ps-2 "
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

          <v-menu open-on-hover>
            <template v-slot:activator="{ props }">
              <v-btn
                color="#216f8c"
                v-bind="props"
                valiant="text"
                class="text-white mr-10"
              >
                services
              </v-btn>
            </template>

            <v-list>
              <v-list-item>
                <v-list-item-title>
                  <NuxtLink
                    to="/tours"
                    class="text-black text-decoration-none text ps-4"
                    >Tours and Travels</NuxtLink
                  >
                </v-list-item-title>
                <v-list-item-title>
                  <NuxtLink
                    to="/hr"
                    class="text-black text-decoration-none text ps-4"
                    >HR Consultancy</NuxtLink
                  >
                </v-list-item-title>
                <v-list-item-title>
                  <NuxtLink
                    to="/hajj"
                    class="text-black text-decoration-none text ps-4"
                    >Hajj Yatra</NuxtLink
                  >
                </v-list-item-title>
              </v-list-item>
            </v-list>
          </v-menu>
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

.nav-color:hover{
  background-color:black;
  color: white;
}

.mb-20 {
  margin-bottom: 80px;
}
.text {
  font-size: 15px;
  margin-right: 12px;
  
}
</style>
