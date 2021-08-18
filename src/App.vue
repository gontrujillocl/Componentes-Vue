<template>
  <div>
    <div><h1 class="text-center text-white my-4">{{mensaje}}</h1></div>
    <Rickymorty></Rickymorty>
  </div>
</template>


<script>
import Rickymorty from "./components/Rickymorty.vue"

export default {
  name:"App",
  data:()=>({
  mensaje: "Desafío - Componentes "
  }),
  components:{
    Rickymorty,
  }
};
</script>