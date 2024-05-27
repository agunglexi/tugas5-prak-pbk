<template>
    <div>
      <b-carousel
        v-if="slides.length"
        v-model="slide"
        controls
        indicators
        background="#ababab"
        img-width="800"
        img-height="400"
        style="text-shadow: 1px 1px 2px #333;"
      >
        <b-carousel-slide
          v-for="(slide, index) in slides"
          :key="index"
          :img-src="slide.imgSrc"
          :caption="slide.caption"
        ></b-carousel-slide>
      </b-carousel>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        slide: 0,
        slides: [
          { imgSrc: 'https://via.placeholder.com/800x400?text=Promotion+1', caption: 'Promotion 1' },
          { imgSrc: 'https://via.placeholder.com/800x400?text=Promotion+2', caption: 'Promotion 2' },
          { imgSrc: 'https://via.placeholder.com/800x400?text=Promotion+3', caption: 'Promotion 3' }
        ]
      };
    }
  }
  </script>
  
  <style scoped>
  /* Custom styling */
  </style>
  