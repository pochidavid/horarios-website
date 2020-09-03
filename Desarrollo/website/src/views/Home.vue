<template>
  <div class="home">
    <div class="titulo">
      E.E.S.T.P.P.I. Nº 8122
      <br>
      "Nuestra Señora de Lourdes"
    </div>
    <div class="subtitulo">
      Sitio Web Horarios 2020
    </div>
    <div class="anuncios">
      <div class="anuncios-titulo">
        Anuncios
      </div>
      <div class="anuncio-content">
        No hay anuncios correspondientes
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>
.home{
  background-color: #f2f2f2;
  height: 100%;
  text-align: center;
  font-family: 'Public Sans';
  padding-top: 5%;
}

.titulo{
  font-size: 40px;
  font-weight: 700;
  padding: 20px;
}

.subtitulo{
  font-size: 32px;
  font-weight: 500;
  padding: 20px;
}

.anuncios{
  padding: 25px;
}

.anuncios-titulo{
  font-size: 24px;
  font-weight: 300;
}

.anuncio-content{
  font-style: italic;
  color: green;
  font-weight: 700;
  font-size: 20px;
}
</style>
