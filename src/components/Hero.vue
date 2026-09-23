<template>
  <div class="hero">
    <div class="hero-text">
        <div><h1>Desarrollador full stack</h1>
        <p>2 años de experiencia en el mundo del desarrollo</p></div>

        <div class="hero-btn"><Button button-text="Ver proyectos"></Button><Button button-text="Github"></Button></div>
        
    </div>
    <div class="hero-img">
        <img class="img-cd" src="../assets/Crypto.png" alt="codigo" />
        <img class="img-bd" src="../assets/bd.png" alt="bd" />
    </div>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  name: 'Hero',
components:{
    Button
},
  data() {
    return {
     
    }
  },

  methods: {
    
  },

  mounted() {
   
  }
}
</script>

<style scoped>
.hero{
    display: flex;
align-items: center;
justify-content: center;
background-color: #42c7c3;
}
.hero-text{
    width: 50%;
    text-align: center;
}

.hero-btn{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 30px;
}

.img-cd{
   z-index: 0;
}

.img-bd{
z-index: 1;
position: absolute;
top: 500px;
left: 180px;
}
</style>