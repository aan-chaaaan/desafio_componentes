<template>
  <div>
    <div v-for="(Personaje, index) of Personajes" :key="index">
      <div class="card-images">
        <img class="image-character" v-bind="Personaje" alt="imagenes" />
        <p>{{ Personaje.nombre }}</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "images",
  data: () => ({
    Personajes: [
      {
        nombre: "Rick Sanchez",
        src: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        nombre: "Morty Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        nombre: "Summer Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        nombre: "Beth Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        nombre: "Jerry Smith",
        src: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
    ],
    background:{
    src: "https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png",
    }
  }),
  
};
</script>

<style scoped lang="scss">
//images debe contener las mismas caracteristicas(misma letra tamaño color y forma circular)
body,
html {
  width: 100%;
  height: 100%;
  box-sizing: border-box;
  margin: 0;
}

.image-character{
  width: 115px;
  border-radius: 50%;
  margin-right: 25px;
}
.card-images{
  color: green;
  font-family: monospace;
  font-size: 30px;
  font-weight: 600; 
}
p{
  width: 50%;
  display: inline-block;
  position: absolute;
  padding-top: 20px;
}
</style>
