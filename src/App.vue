<template>
  <div id="App" :style="image" class="image">
    <images></images>
  </div>
</template>

<script>
import images from "./components/componente.vue";

export default {
  name: "App",
  components: {
    images,
  },
  data(){
    return{
      image:{
        backgroundImage: "url(https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png)"
      }
    }

  }
};
</script>

<style scoped lang="scss">
body,
html {
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  margin: 0;
}
.image {
  background-repeat: no-repeat;
  background-position: top;
  background-size: cover ;
  margin: 0;

}
</style>
