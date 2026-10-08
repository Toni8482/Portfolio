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
  flex-wrap: wrap;
  padding: 15px;
  gap: 50px;
  justify-content: center;
}

.card-text {

  padding: 50px;
  flex-basis: 40%;
}

.card-img {
  display: flex;
  flex-direction: column;
 flex-basis: 55%;
  gap: 30px;
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
  width: 14%;
  margin-top: auto;

}

#img-laptop {
  object-fit: contain;
  width: 84%;
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

@media (max-width: 1382px) {
   .card-text, .card-img {

 
  flex-basis: 95%;
}
}
</style>