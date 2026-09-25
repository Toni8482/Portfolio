

<template>
  <Header/>
  <Hero></Hero>
  <About></About>
  <Skins></Skins>
  <Projects></Projects>
  <Contact></Contact>
  <Footer></Footer>
</template>


<script>
import About from './components/About.vue';
import Header from './components/Header.vue';
import Hero from './components/Hero.vue';
import Skins from './components/Skins.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';



export default {
  name: 'App',
components: {
 Header,
 Hero,
 About,
 Skins,
 Projects,
 Contact,
 Footer
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