<template>

<section class="section d-flex justify-center align-center">
  <div>
 <h1 class="text-center pt-10 text-white Enjoy">Enjoy Your Vacation With Us</h1>
  <p class="text-center pt-5 text-white joy">Tempor erat elitr rebum at clita diam amet diam et eos erat ipsum lorem sit</p>
    </div>
</section>

 <v-container>
   <h1 class="text-center about">About Us</h1>
   <h3 class="text-center">Welcome to Tourist</h3>
  <div>
    <h4 class=" about">Explore Historic Landmarks:</h4>
    <p>Step back in time as you wander through the cobblestone streets of our historic district. Marvel at the architectural wonders of ancient temples, medieval castles, and grand cathedrals. Don't miss the opportunity to visit iconic landmarks such as [Famous Landmark], [Another Famous Landmark], and [Yet Another Famous Landmark].</p>
    <h4 class=" about">Immerse Yourself in Culture:</h4>
    <p>Indulge your senses in [Destination Name]'s vibrant cultural scene. Delve into the local arts and crafts at bustling markets and artisan workshops. Experience the rhythm of traditional music and dance performances that celebrate our heritage. And be sure to sample the flavors of [Destination Name] with a culinary journey through our diverse cuisine, from street food delights to haute cuisine experiences.</p>

    <h4 class=" about">Embrace Nature's Beauty:</h4>
    <p>Embark on an adventure into the great outdoors and discover [Destination Name]'s natural wonders. Hike through lush rainforests, where exotic wildlife and cascading waterfalls await around every corner. Relax on pristine beaches with golden sands and crystal-clear waters, perfect for swimming, snorkeling, or simply soaking up the sun. Explore rugged mountains and serene lakes, offering breathtaking vistas and endless opportunities for outdoor recreation.</p>
  </div>
<h4 class="vision mt-10">Our Vision</h4>
  <v-row>
    <v-col cols="12" lg="4">
      <v-card class="card pa-3">
          <div class="box">
            <Icon name="fluent:building-bank-20-regular" style="font-size: 24px;" />
          </div>
          <h5 class="mt-6">Mission</h5>
          <p>We aim to make the world a better place through innovation and collaboration.</p>
      </v-card>
    </v-col>
    <v-col cols="12" lg="4">
        <v-card class="card pa-3">
          <div class="box">
            <Icon name="ph:graduation-cap-light" style="font-size: 22px;" />
          </div>
          <h5 class="mt-6">Values</h5>
          <p>We believe in honesty, integrity, and respect for all individuals.</p>
      </v-card>
    </v-col>
    <v-col cols="12" lg="4">
        <v-card class="card pa-3">
          <div class="box">
            <Icon name="ph:eye" style="font-size: 22px;"  class="" />
          </div>
          <h5 class="mt-6">Vision</h5>
          <p>We envision a world where technology is used to solve the most pressing issues facing humanity and improve people's lives.</p>
      </v-card>
    </v-col>
  </v-row>

  <div class="my-16">
    <h4 class="vision mt-10">Mission</h4>
    <p>Welcome to Mission, California, a quaint yet vibrant town nestled in the heart of the Golden State! As you embark on your journey through this charming locale, you'll discover a delightful blend of history, culture, and natural beauty. From captivating historic sites to picturesque outdoor spaces, Mission offers something for every traveler seeking an authentic Californian experience.</p>
    <p>Begin your adventure by immersing yourself in Mission's rich history. Visit the iconic Mission San Gabriel Arcángel, founded in 1771, one of the oldest and most well-preserved missions in California. Wander through its serene courtyards, marvel at its Spanish colonial architecture, and learn about its significant role in shaping the region's cultural heritage.

</p>
<p>Afterward, step back in time with a stroll through Mission's charming downtown area, where historic buildings and landmarks abound. Stop by the San Gabriel Historical Museum to delve deeper into the town's past, or simply wander the streets lined with quaint shops and eateries, each with its own story to tell.</p>
  </div>
 </v-container>
</template>

<style scoped>
.Enjoy{
  font-size: 60px;
  font-weight: bold;
  padding-top: 100px;
}
.joy{
  font-size: 19px;

}
.section{
     background-image: url("/assets/image/section/section1-banner.jpg");
    /* height: 600px; */
    box-shadow: inset 0 0 0 1000px rgba(0, 0, 0, 0.7);
    min-height: 600px;
    max-width: 100%;
    background-size: cover;
    background-repeat: no-repeat;
}

.box{
  width: 40px;
  height: 40px;
  background-color: #216f8c;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 3px;
  border-radius: 5px;
}

.card{
  height: 200px;
  margin-block: 30px;
}

.vision{
  font-size: 25px;
  font-weight: bold;
}

.about{
  color:#216f8c;
}

</style>