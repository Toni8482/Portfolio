<template>
  <div class="section-projects">

    <div class="card-projects">
      <div class="projects-title">
        <h3>Proyectos</h3>
      </div>
      <Card></Card>
      <Card></Card>
      <Card></Card>
    </div>
  </div>
</template>

<script>

import Card from "./Card.vue";

export default {
  name: 'Projects',
  components: {
    Card
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
.section-projects {
  padding: 80px;
}

.projects-title {
  background-color: var(--surface);
  border: solid;
  border-color: var(--boder);
  border-radius: 15px;
  padding: 10px;
  top: 40px;
  right: -50px;
  position: absolute;
  height: fit-content;
  width: fit-content;
  box-shadow: 5px 12px;
  font-size: x-large;
  background-color: #ffffff;

}

.card-projects {

  background-color: var(--accent);
  border: solid;
  border-radius: 30px;
  display: flex;
  flex-direction: column;
  padding: 80px;
  gap: 30px;
  position: relative;
}
</style>