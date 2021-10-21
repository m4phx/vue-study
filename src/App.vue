<template>
    <div>
      <h1> {{ titulo }} </h1>
      <ul> 
      <li v-for="foto of fotos">
        <img :src="foto.url" :alt="foto.titulo">
      </li>
      </ul>
  </div>
</template>

<script>

export default {
  name: 'app',
  data () {
    return {
     titulo: 'Alurapic',
     fotos: [
       {
        url: 'https://exame.com/wp-content/uploads/2017/05/darpa-boeing.jpg',
        titulo: 'foguete'
       },
       {
        url: 'https://exame.com/wp-content/uploads/2017/05/darpa-boeing.jpg',
        titulo: 'foguete2'
       }
     ]
    }
  }
}

</script>

<style>

</style>
