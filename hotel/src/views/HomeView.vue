<template>
  <div class="home">
    <div class="landing-photo">
      <img src="../assets/landingphoto.png" alt="Landing Photo" />
      <div class="centered-text">
        <h2>Enjoy Your Dream Vacation</h2>
        <h4>Plan and book our perfect trip with expert advice, travel tips, destination information and inspiration from us</h4>
      </div>
    </div>
    <div class="search">
      <SearchBar />
    </div>
  </div>
</template>
    

  <script>
  // @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import SearchBar from '@/components/SearchBar.vue';

  export default {
    name: 'HomeView',
    components: {
    HelloWorld,
    SearchBar
}
  }
  </script>

<style>

.home {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  height: 100vh;
}

.landing-photo img {
  width: 100%;
  height: auto;
  display: block;
  margin-top: 10px;
}

.centered-text {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  color: white;
  font-size: 24px;
  text-align: center;
}
  </style>
