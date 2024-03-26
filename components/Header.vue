<script setup>
let drawer = ref(false);
</script>

<template>
  <!-- for large screen -->
  <div class="d-flex justify-between align-center header">
    


<div class="mt-4">
  <a href="/" class="link mr-10">Home</a>
  <a href="/contact" class="link mr-10">Contact</a>
</div>
 
  </div>
</template>

<style>
.d-flex.align-center {
  align-items: center;
}

.input {
  flex: 1;
  /* Adjust as needed */
  max-width: 500px;
}

.v-btn {
  color: #333;
  font-size: 14px;
  padding: 10px;
}

.v-btn.icon p {
  margin: 0;
  font-size: 14px;
}
.wisdom{
  font-weight: bold;
  font-size: 20px;
}

.link{
  color: black;
  font-size: 20px;
  text-decoration: none;

}
.link:hover{
  color: green;
  text-decoration: underline;
}
.header{
  border-bottom: 2px solid green;
}
</style>
