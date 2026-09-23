<template>
    <div class="header">

        <!-- LOGO -->

        <div><img src="../assets/Code.png" alt="Logo"></div>

        <!-- NAV-BAR -->

        <div>
            <ul>
                <li><a href="">Inicio</a></li>
                <li><a href="">Sobre mi</a></li>
                <li><a href="">Tegnologias</a></li>
                <li><a href="">Proyectos</a></li>
                <li><a href="">Contacto</a></li>
            </ul>
        </div>

        <!-- DESCARGA CV -->

        <div><Button button-text="Descargar CV"></Button></div>
    </div>
</template>

<script>
import Button from "./Button.vue";

export default {
    name: 'Header',
    components: {
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
.header {
    display: flex;
    width: 100%;
    background-color:transparent;
    align-items: center;
    justify-content: space-between;
    padding: 0px 30px 0px 30px;
    box-sizing: border-box;
}


.header ul {
    display: flex;
    list-style: none;
    gap: 40px;
}

.header ul a {
    color: black;
    text-decoration: none;
}


.header ul a:hover {
    color: rgb(173, 120, 120);
   
}

</style>