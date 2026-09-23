

<template>
  <Header/>
  <Hero></Hero>
  <About></About>
</template>


<script>
import About from './components/About.vue';
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';



export default {
  name: 'App',
components: {
 Header,
 Hero,
 About
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