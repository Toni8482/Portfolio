<template>
  <div class="tag">
   <span>{{ textTag }}</span>
  </div>
</template>

<script>
export default {
  name: 'Tag',
props:{
textTag:String
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
.tag{
    background-color: black;
    border: solid;
    border-color: var(--border);
    border-radius: 50px;
    color: aliceblue;
    padding: 10px;
}
</style>