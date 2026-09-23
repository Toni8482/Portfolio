<template>
  <div>
   
    <button @click="saludar">{{ buttonText }}</button>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props:{
    buttonText:String
  },

  data() {
    return {
     
    }
  },

  methods: {
    saludar() {
      console.log('¡Hola!')
    }
  },

  mounted() {
   
  }
}
</script>

<style scoped>

button{
    background-color:var(--accent);
    color: black;
    border-radius: 15px;
    padding:0 12px 0 12px;
    border-color: black;
    cursor: pointer;
}
</style>