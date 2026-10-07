<template>
    <div class="header">

        <!-- LOGO -->

        <div><img src="../assets/Code.png" alt="Logo"></div>

        <!-- NAV-BAR -->

        <div class="nav-bar">
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#sobre_mi">Sobre mí</a></li>
                <li><a href="#tecnologias">Tecnologías</a></li>
                <li><a href="#proyectos">Proyectos</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </div>

        <!-- DESCARGA CV -->

        <div class="section-download-cv"><Button class="btn-cv" button-text="Descargar CV" :icon_path=icon_path
                @init-button="downloadCV"></Button></div>

        <!-- NAV-BAR-PHONE -->

        <div class="menu-phone">
            <button class="nav-phone" @click="desplegarMenuPhone">
                <img src="../assets/sandwich.png" alt="sandwich">
            </button>

            <div class="menu-desplegable" :class="[desplegable ? 'desactivado' : 'activado']">
                <ul>
                    <li><a href="#inicio">Inicio</a></li>
                    <li><a href="#sobre_mi">Sobre mí</a></li>
                    <li><a href="#tecnologias">Tecnologías</a></li>
                    <li><a href="#proyectos">Proyectos</a></li>
                    <li><a href="#contacto">Contacto</a></li>
                </ul>
            </div>
        </div>
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
            desplegable: false,
            icon_path: '../src/assets/Download.svg',
            downloadPath: '../src/assets/cv.pdf'
        }
    },

    methods: {


        desplegarMenuPhone() {
            if (this.desplegable) {
                this.desplegable = false;

                console.log(this.desplegable);
            }
            else {
                this.desplegable = true;
                console.log(this.desplegable);
            }
        },

        /* DESCARGAR CURRICULUM */

        downloadCV(init) {
            console.log(init);
            let resultConfirm = confirm("Descargar curriculum");
            if (resultConfirm) {
                const enlace = document.createElement("a");
                enlace.href = this.downloadPath;
                enlace.download = "Toni_Tirado_CV.pdf";
                enlace.click();
            }
        }

    },

    mounted() {

    }
}
</script>

<style scoped>
.header {
    display: flex;
    width: 100%;
    background-color: transparent;
    align-items: center;
    justify-content: space-between;
    padding: 0px 30px 0px 30px;
    box-sizing: border-box;
    position: relative;
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

.menu-phone,
.nav-phone {
    display: none;
}

.menu-desplegable {
    display: none;
    position: absolute;
    top: 100%;
    left: 0;
    background-color: bisque;
    width: 100%;
    transition: all 1s;
    overflow: hidden;
}

.menu-desplegable ul {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

}

.btn-cv {

    font-weight: 600;
}

@media (max-width: 1024px) {}


@media (max-width: 768px) {

    .nav-bar {
        display: none;

    }

    .section-download-cv {
        display: none;
    }


    .menu-phone {
        display: block;
    }

    .nav-phone {
        display: flex;
        background-color: var(--accent);
        border: solid 1px;
        border-radius: 5px;
        border-color: var(--border);
    }

    .menu-desplegable {
        display: block;
        z-index: 10;
    }


    .menu-desplegable.desactivado {

        max-height: 0;
    }

    .menu-desplegable.activado {
        max-height: 100vh;

    }

}
</style>