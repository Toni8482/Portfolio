<template>
    <div class="about">
        <div class="about-div">
            <div class="about-title-img">
                <div class="about-img"><img src="../assets/yo.png" alt="perfil"></div>
                <div class="about-title">
                    <h3>Sobre mi</h3>
                </div>

            </div>

            <div class="about-text">
                <p>Soy desarrollador Full Stack con varios años de experiencia dedicándome al desarrollo de aplicaciones
                    web.</p>

                <p>Me gusta involucrarme en todo el proceso de desarrollo, desde entender una idea y definir cómo
                    llevarla a cabo, hasta diseñar su arquitectura, desarrollar el frontend y backend, desplegar la
                    aplicación y mantenerla a lo largo del tiempo.</p>

                <p>Para mí, desarrollar software no consiste únicamente en escribir código. Me interesa entender el
                    problema que hay detrás, conocer cómo funcionan las diferentes partes de una aplicación y encontrar
                    soluciones que sean sencillas, eficientes y mantenibles.</p>

                <p>Siempre intento seguir aprendiendo y descubrir nuevas formas de hacer mejor las cosas, tanto a nivel
                    técnico como en la forma de afrontar un proyecto.</p>
            </div>
            <div class="about-tags">

                <Tag text-tag="Trabajo"></Tag>
                <Tag text-tag="Aprendiendo"></Tag>
                <Tag text-tag="Frondtend"></Tag>
                <Tag text-tag="Backend"></Tag>
            </div>


        </div>
    </div>
</template>

<script>
import Tag from "./Tags.vue";

export default {
    name: 'About',
    components: {
        Tag
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
.about {
    padding: 150px 0 50px;
    display: flex;
    justify-content: center;
}

.about-div {
    display: flex;
    flex-direction: column;
    background-color: var(--surface);
    border: solid 1px;
    border-radius: 30px;
    border-color: var(--border);
    width: 70%;
    padding: 50px;
    position: relative;
}

.about-title-img {
    position: absolute;
    top: -85px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 90%;

}

.about-title {
    padding: 15px;
    background-color: #ffffff;
    border: solid 1px;
    border-radius: 15px;
    border-color: var(--border);


    height: fit-content;
    box-shadow: 5px 12px;
    font-size: x-large;
}

.about-img {}

.about-text {

    padding: 40px 0 30px 0;
}

.about-tags {
    display: flex;
    gap: 30px;
    justify-content: center;
}


@media (max-width: 1024px) {
 
}


@media (max-width: 768px) {
  
.about-title-img {
   flex-direction: column-reverse;
   gap: 30px;
 top: -25px;
   width: auto;
}
.about-text {

    padding: 180px 0 30px 0;
}


.about-tags {
   display: grid;
   grid-template-columns: 1fr 1fr;
}

.about-tags {
  text-align: center;
}
}
</style>