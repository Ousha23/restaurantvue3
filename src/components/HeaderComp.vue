<template  >
  <header>
    <div id="bg-color"></div>
    <div id="bg-image">
      <NavBar />
      <TitleDescover />
      <div id="triangle"></div>
    </div>
  </header>
    
</template>
  
  <style scoped>
   #triangle {
        width: 0px;
        height: 0px;
        border-style: solid;
        border-width: 0 0 300px 2000px;
        border-color: transparent transparent rgb(43, 43, 43) transparent;
        transform: rotate(4deg);
        position: absolute;
        left: 0;
        bottom: -15%;
    }
    #bg-color {
      background-color: rgb(85, 85, 164);
      width: 100%;
      height: 50vh;
      position: absolute;
      z-index: -1;
  }
    #bg-image {
      background-image:url("@/assets/img/splashscreen.jpg");
      background-position: center;
      background-size: cover;
      width: 100%;
      height: 50vh;
    }
    header {
      position: relative;
      overflow: hidden;
    }
  
  </style>
  
  <script setup>
  // @ is an alias to /src
  import NavBar from '@/components/NavBar.vue'
  import TitleDescover from '@/components/TitleDescover.vue';
  
  </script>
  