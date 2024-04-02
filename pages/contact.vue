<script setup>
let name = ref('')
let email= ref('')
let subject = ref('')
let message = ref('')

async function sendMail() {
  try {
    let res = await fetch("http://localhost:5000/api/contacts", {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json'
      },
      body: JSON.stringify({
        name: name.value,
        email: email.value,
        subject: subject.value,
        message: message.value
      })
    });

    if (res.ok) {
      console.log('Email sent successfully');
    } else {
      console.error('Failed to send email');
    }
  } catch (error) {
    console.error('Error sending email',);
  }

  name.value = ''
  email.value = ''
  subject.value = ''
  message.value = ''
}

</script>


<template>
  <section class="section d-flex justify-evenly align-center">
    <div>
      <h1 class="text-center pt-10 text-white Enjoy">CONTACT US</h1>
    </div>
  </section>

  <v-container>
    <section class="section2 my-16">
      <p class="text-center contact mb-0">CONTACT US</p>
      <h2 class="text-center mb-16 contact2">Contact For Any Query</h2>
      <v-row>
        <v-col>
          <p class="mb-0 get">Get In Touch</p>
          <p>
            Tempor erat elitr rebum at clita. Diam dolor diam ipsum sit. Aliqu
            diam amet diam et eos
          </p>

          <div class="d-flex">
            <div class="box mr-5">
              <Icon name="mdi:location" style="font-size: 22px" class="mb-3" />
            </div>
            <div>
              <p class=" mb-0 office">Office</p>
              <p>123 Street, New York, USA</p>
            </div>
          </div>

          <div class="d-flex">
            <div class="box mr-5">
              <Icon
                name="solar:phone-bold"
                style="font-size: 22px"
                class="mb-3"
              />
            </div>
            <div>
              <p class=" mb-0 office">Mobile</p>
              <p>+012 345 67890</p>
            </div>
          </div>

          <div class="d-flex">
            <div class="box mr-5">
              <Icon name="mdi:email" style="font-size: 22px" class="mb-3" />
            </div>
            <div>
              <p class=" mb-0 office">Email</p>
              <p>info@example.com</p>
            </div>
          </div>
        </v-col>

        <v-col>
          <div>
            <div class="d-flex">
              <v-text-field
                label="Your Name"
                variant="outlined"
                class="mr-2"
                v-model="name"
              ></v-text-field>
              <v-text-field
                label="Your Email"
                variant="outlined"
                v-model="email"
              ></v-text-field>
            </div>
            <v-text-field label="Subject" v-model="subject" variant="outlined"></v-text-field>
            <v-textarea label="Message" v-model="message" variant="outlined"></v-textarea>
            <v-btn class=" btn" @click="sendMail()"> Send Message </v-btn>
          </div>
        </v-col>
      </v-row>
    </section>
  </v-container>
</template>

<style scoped>
.section {
  background-image: url('/assets/image/section/section1-banner2.jpg');
  /* height: 600px; */
  box-shadow: inset 0 0 0 1000px rgba(0, 0, 0, 0.7);
  min-height: 600px;
  max-width: 100%;
  background-size: cover;
  background-repeat: no-repeat;
}

.box {
  width: 50px;
  height: 50px;
  background-color: #216f8c;
  color: white;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.get {
  font-weight: bold;
  font-size: 20px;
}
.office {
  font-size: 20px;
  font-weight: bold;
  color: black;

}

.contact {
  color: #216f8c;
  font-size: 25px;
  font-weight: bold;
}

.btn {
  width: 600px;
  background-color: #216f8c;
  color: white;
}
.contact2 {
  font-weight: bold;
  font-size: 40px;
  color: rgb(86, 85, 85);
}
</style>
