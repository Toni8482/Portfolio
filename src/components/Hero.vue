<template>
  <div class="hero">
    <div class="hero-text">
      <div>
        <h1>Desarrollador full stack</h1>
        <p>2 años de experiencia en el mundo del desarrollo</p>
      </div>

      <div class="hero-btn">
        <Button class="btn" button-text="Ver proyectos" :icon_path=icon_path_proyectos @init-button="proyectos">
        </Button>

        <Button class="btn" button-text="Contactame" :icon_path=icon_path_github @init-button="contactame">
        </Button>
      </div>

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
  components: {
    Button
  },
  data() {
    return {
      icon_path_proyectos: '../src/assets/Laptop.svg',
      icon_path_github: '../src/assets/sobre.svg',
    }
  },

  methods: {

    /* METODOS PARA ACCIÓN DE BOTONES */
    proyectos() {

      const enlace = document.createElement("a");
      enlace.href = '#proyectos';
      enlace.click();

    },
    contactame() {

      const enlace = document.createElement("a");
      enlace.href = "#contacto";
      enlace.click();
    }

  },

  mounted() {

  }
}
</script>

<style scoped>
.hero {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #42c7c3;

}

h1 {
  font-size: 50px;
  margin-bottom: 20px;
}

.hero-text {
  width: 50%;
  text-align: center;
  display: flex;
  flex-direction: column;
  gap: 30px;
}

.hero-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 30px;
}

.hero-img {
  position: relative;
  overflow: hidden;
  width: 50%;
  height: stretch;
}

.img-cd {
  width: 100%;
  height: 100%;
  z-index: 0;
  object-fit: fill;
}

.img-bd {
  width: 80%;

  z-index: 1;
  position: absolute;
  top: 60%;
  right: 20%;
}

.btn {
  padding: 10px;
  display: flex;
  font-weight: 600;
  gap: 10px;
}


@media (max-width: 1024px) {
  h1 {
    font-size: 40px;
    margin-bottom: 20px;
  }
}


@media (max-width: 768px) {
  .hero {
    flex-direction: column;
    padding: 50px 0 0 0;
  }

  h1 {
    font-size: 30px;
    margin-bottom: 10px;
  }

  .hero-text {
    width: 100%;

  }

  .hero-img {
    width: 100%;
  }

}
</style>