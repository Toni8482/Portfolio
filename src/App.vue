

<template>
  <Header/>
  <Hero></Hero>
  <About></About>
  <Skins></Skins>
</template>


<script>
import About from './components/About.vue';
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Skins from './components/Skins.vue';



export default {
  name: 'App',
components: {
 Header,
 Hero,
 About,
 Skins
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