<template>
  <div class="card">
    <div class="card-text">

      <h3>Scraper perfumes</h3>
      <p>
        Es una app que scrapea varias tiendas de perfume y recgoge sus datos para comprar los perfumes en distintas
        tiendas
      </p>
      <div class="card-buttons">
        <Button class="btn-card" button-text="Sitio web"></Button>
        <Button class="btn-card" button-text="Github"></Button>
      </div>
    </div>
    <div class="card-img">
      <div class="imgs-projects">
        <img id="img-phone" src="../assets/phone.png" alt="phone">
        <img id="img-laptop" src="../assets/laptop.png" alt="laptop">
      </div>
      <div class="tags-projects">

        <Tag text-tag="Javascript"></Tag>
        <Tag text-tag="PHP"></Tag>
        <Tag text-tag="MySql"></Tag>
      </div>

    </div>

  </div>
</template>

<script>
import Tag from "./Tags.vue";
import Button from "./Button.vue";


export default {
  name: 'Card',
  components: {
    Tag,
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
.card {


  background-color: var(--surface);
  border-radius: 15px;
  border: solid;
  display: flex;

  padding: 50px;
  gap: 50px;
}

.card-text {

  padding: 50px;
  width: 45%;
}

.card-img {
  display: flex;
  flex-direction: column;
  
  gap: 40px;
}

.imgs-projects {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 10px;

}

.tags-projects {

  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
}

#img-phone {
 object-fit: contain;
 width: 15%;
   margin-top: auto;
 
}

#img-laptop { object-fit: contain;
width: 80%;
  margin-top: auto;
}

.card-buttons {
  display: flex;
  gap: 10px;
}

.btn-card {
font-size: large;
font-weight: bold;
  padding: 10px;
}
</style>