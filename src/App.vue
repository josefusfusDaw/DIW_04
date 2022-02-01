<template>
  <encabezado msg="Welcome to Your Vue.js App" />
  <div class="container">
    <migas />
    <div class="estilocuerpo">
       <cuerpoizq />
      <cuerpo msg="Welcome to Your Vue.js App" />
     
    </div>
  </div>
  <pie msg="Welcome to Your Vue.js App" />
</template>

<script>
import encabezado from "./components/encabezado.vue";
import cuerpo from "./components/cuerpo.vue";
import pie from "./components/pie.vue";
import cuerpoizq from "./components/cuerpoizq.vue";
import migas from "./components/caminomigas.vue";

export default {
  name: "App",
  components: {
    encabezado,
    cuerpo,
    pie,
    cuerpoizq,
    migas
  },
};
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  background-color: #fffbfb;;
}

#app {
  font-family: "Titillium Web", sans-serif;
}

.container {
  /*max-width: 1400px;*/
  margin: auto;
}

.estilocuerpo {
  display: flex;
  margin: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
