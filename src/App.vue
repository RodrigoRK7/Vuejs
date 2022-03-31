<template>
  <BotonMenu/>
  <Mascotas msg="BIENVENIDOS A MASCOTAS"/>
  <Slider :slides="slides" :interval="3000" controls indicators></Slider>
  <Card/>
</template>

<script>
import Mascotas from './components/Mascotas.vue'
import BotonMenu from './components/BotonMenu.vue'
import Slider from "./components/SliderCarousel.vue";
import Card from "./components/CardComponent.vue"

export default {
  name: 'App',
  components: {
    Mascotas,
    BotonMenu,
    Slider,
    Card
  },
  data:()=>({
    slides: [
      "https://cdn.pixabay.com/photo/2021/09/10/20/02/cats-6614088__340.jpg",
      "https://cdn.pixabay.com/photo/2017/08/29/01/22/dog-2691871__340.jpg",
      "https://cdn.pixabay.com/photo/2021/09/17/10/55/caiman-lizard-6632344__340.jpg",
      "https://cdn.pixabay.com/photo/2018/03/29/21/51/cute-3273789__340.jpg",
      "https://cdn.pixabay.com/photo/2016/11/29/08/31/animal-1868436__340.jpg",
      "https://cdn.pixabay.com/photo/2016/10/26/22/00/hamster-1772742__480.jpg",
      "https://cdn.pixabay.com/photo/2022/03/03/10/18/birds-7045043__340.jpg"
    ]
  })
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.espacio{
  padding: 15px;
}
</style>
