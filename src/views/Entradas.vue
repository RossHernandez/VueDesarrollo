<template>
<div>
  <v-carousel :show-arrows="false" height="450" float="left">
    <v-carousel-item class="carousel"
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
    ></v-carousel-item>
  </v-carousel>
  </div>
</template>
<script>
export default {
  data() {
    return {
      bottomNav: 'recent',
      drawer: null,
      items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
          {
            src: 'https://laopinion.com/wp-content/uploads/sites/3/2016/09/chilesennogada.jpg?quality=80&strip=all',
          },
        ],
    }
  },
}
</script>
<style>
.carousel {
    overflow: hidden;
    position: relative;
    width: 60%;
    display: block;
    margin:  auto;
    /*float: left;*/ 
    
}

</style>