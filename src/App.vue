

<template>
  <Header/>
  <Hero></Hero>
  <About></About>
  <Skins></Skins>
  <Projects></Projects>
</template>


<script>
import About from './components/About.vue';
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Skins from './components/Skins.vue';
import Projects from './components/Projects.vue';



export default {
  name: 'App',
components: {
 Header,
 Hero,
 About,
 Skins,
 Projects
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