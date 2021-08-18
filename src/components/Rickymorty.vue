<template>
   <div class="container">
      <table class="table table-dark">
      <tbody>
         <tr v-for="(perfil, index) in personajes" :key="index">
            <th scope="row"><img v-bind:src="perfil.src" alt="Personajes"></th>
            <td class="name-text">👉{{perfil.nombre}}</td>
         </tr>
      </tbody>
      </table>
   </div>
</template>

<script>
export default {
   name:"Rickymorty",
   data:()=>({
     personajes:[

       {nombre:"Rick Sanchez", 
       src:"https://rickandmortyapi.com/api/character/avatar/1.jpeg"},
       {nombre:"Morty Smith", 
       src:"https://rickandmortyapi.com/api/character/avatar/2.jpeg"},
       {nombre:"Summer Smith", 
       src:"https://rickandmortyapi.com/api/character/avatar/3.jpeg"},
       {nombre:"Beth Smith", 
       src:"https://rickandmortyapi.com/api/character/avatar/4.jpeg"},
       {nombre:"Jerry Smith", 
       src:"https://rickandmortyapi.com/api/character/avatar/5.jpeg"}
   ]
   })
};
</script>

<style>
   img{
      width: 65px;
      border-radius: 50%;
   }

   .name-text{
      font-size: 25px;
      color:green;
   }

   th{
      width: 30px;
   }
   
   body{
      background-image: 
      url("https://rickandmortypod.com/wp-content/uploads/2018/11/cropped-RM_page-header_background1-3.png");
   }
</style>