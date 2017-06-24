<template>
  <div>
    <h1>{{ titulo }}</h1>
    <ul>
      <li v-for="foto of fotos">
        <img :src="foto.url" :alt="foto.titulo">
      </li>
    </ul>
  </div>
</template>

<script>
  export default { 
    data() {
      return {
        titulo: 'Alurapic',
        fotos: [
          {
            url: 'http://portaldodog.com.br/cachorros/wp-content/uploads/2015/06/husky-siberiano-10-500x375.jpg',
            titulo: 'cachorro'
          },
          {
            url: 'http://portaldodog.com.br/cachorros/wp-content/uploads/2015/06/husky-siberiano-10-500x375.jpg',
            titulo: 'cachorrao'
          }
        ]
      }
    }
  }
</script>

<style>
</style>