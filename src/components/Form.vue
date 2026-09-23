<template>
  <div>
    {{ mensaje }}
    <button @click="saludar">Saludar</button>
  </div>
</template>

<script>
export default {
  name: 'MiComponente',

  data() {
    return {
      mensaje: 'Hola mundo'
    }
  },

  methods: {
    saludar() {
      console.log('¡Hola!')
    }
  },

  mounted() {
    console.log('Componente montado')
  }
}
</script>

<style scoped>
</style>