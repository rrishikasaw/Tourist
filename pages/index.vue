<script setup>
import image1 from '../assets/image/section/section1-banner.jpg';
import image2 from '../assets/image/section/section1-banner2.jpg';
import image3 from '../assets/image/section/section-banner3.jpg';
</script>

<template>
    
  <section class="d-flex justify-center align-center">
 
    <!-- <div>
 <h1 class="text-center pt-10 text-white Enjoy">Enjoy Your Vacation With Us</h1>
  <p class="text-center pt-5 text-white joy">Tempor erat elitr rebum at clita diam amet diam et eos erat ipsum lorem sit</p>
    </div> -->

    <v-carousel>
      <v-carousel-item :src="image1" cover></v-carousel-item>

      <v-carousel-item :src="image2" cover></v-carousel-item>

      <v-carousel-item :src="image3" cover></v-carousel-item>
    </v-carousel>
  </section>
  <v-container>
    <section class="section2 mt-10">
      <v-row>
        <v-col>
          <img
            src="../assets/image/section2-image.webp"
            alt=""
            class="w-full"
            height="350"
          />
        </v-col>
        <v-col>
          <p class="mb-0">ABOUT US</p>
          <h3 class="font-bold welcome">
            Welcome to <span class="tourist">Tourist</span>
          </h3>
          <p>
            Tempor erat elitr rebum at clita. Diam dolor diam ipsum sit. Aliqu
            diam amet diam et eos. Clita erat ipsum et lorem et sit.
          </p>
          <p>
            Tempor erat elitr rebum at clita. Diam dolor diam ipsum sit. Aliqu
            diam amet diam et eos. Clita erat ipsum et lorem et sit, sed stet
            lorem sit clita duo justo magna dolore erat amet
          </p>
          <div class="d-flex justify-between">
            <div>
              <div class="d-flex">
                <Icon
                  name="dashicons:arrow-right"
                  style="font-size: 28px"
                  class="mb-3 icon"
                />
                <p class="mb-0">First Class Flights</p>
              </div>
              <div class="d-flex">
                <Icon
                  name="dashicons:arrow-right"
                  style="font-size: 28px"
                  class="mb-3 icon"
                />
                <p class="mb-0">5 Star Accommodations</p>
              </div>
              <div class="d-flex">
                <Icon
                  name="dashicons:arrow-right"
                  style="font-size: 28px"
                  class="mb-3 icon"
                />
                <p class="mb-0">150 Premium City Tours</p>
              </div>
            </div>
            <div>
              <div class="d-flex">
                <Icon
                  name="dashicons:arrow-right"
                  style="font-size: 28px"
                  class="mb-3 icon"
                />
                <p class="mb-0">Handpicked Hotels</p>
              </div>

              <div class="d-flex">
                <Icon
                  name="dashicons:arrow-right"
                  style="font-size: 28px"
                  class="mb-3 icon"
                />
                <p class="mb-0">Latest Model Vehicles</p>
              </div>

              <div class="d-flex">
                <Icon
                  name="dashicons:arrow-right"
                  style="font-size: 28px"
                  class="mb-3 icon"
                />
                <p class="mb-0">24/7 Service</p>
              </div>
            </div>
          </div>
        </v-col>
      </v-row>
    </section>

    <section class="my-16">
      <p class="text-center mb-0 titles">SERVICES</p>
      <h3 class="text-center">Our Services</h3>
      <v-row>
        <v-col cols="12" lg="4">
          <v-card
            class="card2 pa-10"
            style="box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3)"
          >
            <Icon
              name="pajamas:earth"
              style="font-size: 40px"
              class="mb-3 icon"
            />
            <h5>Tours and Travels</h5>
            <p>
              Diam elitr kasd sed at elitr sed ipsum justo dolor sed clita amet
              diam
            </p>
          </v-card>
        </v-col>

        <v-col cols="12" lg="4">
          <v-card
            class="card2 pa-10"
            style="box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3)"
          >
            <Icon
              name="fa-solid:building"
              style="font-size: 40px"
              class="mb-3 icon"
            />
            <h5>HR Consultancy</h5>
            <p>
              Diam elitr kasd sed at elitr sed ipsum justo dolor sed clita amet
              diam
            </p>
          </v-card>
        </v-col>

        <v-col cols="12" lg="4">
          <v-card
            class="card2 pa-10"
            style="box-shadow: 0 4px 6px rgba(0, 0, 0, 0.3)"
          >
            <Icon name="oi:person" style="font-size: 40px" class="mb-3 icon" />
            <h5>Ummarh and hajj</h5>
            <p>
              Diam elitr kasd sed at elitr sed ipsum justo dolor sed clita amet
              diam
            </p>
          </v-card>
        </v-col>
      </v-row>
    </section>

    <Package />
  </v-container>
</template>

<style scoped>
.section {
  background-image: url('/assets/image/banner.png');
  /* height: 600px; */
  /* box-shadow: inset 0 0 0 1000px rgba(0, 0, 0, 0.8); */
  min-height: 600px;
  max-width: 100%;
  background-size: cover;
  background-repeat: no-repeat;
}
.card2:hover {
  background-color: rgb(173, 173, 243);
  color: white;
}
.titles {
  color: #216f8c;
}
.icon {
  color: #216f8c;
}
.tourist {
  color: #216f8c;
}
.icon {
  color: #216f8c;
}
.icon:hover {
  color: white;
}

.welcome {
  font-weight: bold;
}

.card2 {
  height: 230px;
}

.Enjoy {
  font-size: 50px;
  font-weight: bold;
  padding-top: 100px;
}
.joy {
  font-size: 19px;
}
</style>
