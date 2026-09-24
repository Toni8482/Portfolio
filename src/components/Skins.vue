<template>
  <div class="skins"> <div class="skins-title">
        <h3>Tegnologias</h3>
      </div>
    <div class="skins-section">
     
    
        <div class="skins-card">
          
          <div class="card-title">

  <img src="../assets/Vector.svg" alt="icon">
          <h3> Backend</h3>
        </div>
         
          <div class="card-logos">
            <div> <img src="../assets/logos/logos_mysql.png" alt="MySql">
              <span>Mysql</span>
            </div>
            <div> <img src="../assets/logos/logos_php.png" alt="PHP">
              <span>PHP</span>
            </div>
            <div> <img src="../assets/logos/logos_symfony.png" alt="Symfony">
              <span>Symfony</span>
            </div>
            <div><img src="../assets/logos/logos_java.png" alt="Java"><span>Java</span></div>
          </div>
        </div>
        <div class="skins-card">

            <div class="card-title">

  <img src="../assets/Monitor.svg" alt="icon">
        <h3>Frontend</h3>
        </div>
         
          <div class="card-logos">
            <div> <img src="../assets/logos/logos_html-5.png" alt="Html">
              <span>Html</span>
            </div>
            <div> <img src="../assets/logos/devicon_css.png" alt="CSS3">
              <span>CSS3</span>
            </div>
            <div> <img src="../assets/logos/logos_javascript.png" alt="JavaScript">
              <span>Javascript</span>
            </div>
            <div> <img src="../assets/logos/logos_vue.png" alt="Vue">
              <span>Vue</span>
            </div>
          </div>
        </div>
        <div class="skins-card">

            <div class="card-title">

 <img src="../assets/Tools.svg" alt="icon">
          <h3>Herramientas</h3>
        </div>
        
          <div class="card-logos">
            <div> <img src="../assets/logos/devicon_git-wordmark.png" alt="Git">
              <span>Git</span>
            </div>
            <div> <img src="../assets/logos/logos_github-icon.png" alt="Github">
              <span>Github</span>
            </div>
            <div> <img src="../assets/logos/devicon_figma.png" alt="Figma">
              <span>Figma</span>
            </div>
            <div><img src="../assets/logos/logos_docker-icon.png" alt="Docker">
              <span>Docker</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  
</template>

<script>
export default {
  name: 'Skins',

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
.skins {
  padding: 30px 0 30px;
}
.card-title{
 display: flex;
 gap: 10px;
}
.skins-title {
  background-color: var(--surface);
  border: solid;
  border-color: var(--boder);
  border-radius: 15px;
  padding: 10px;
  top: 40px;
  right: -150px;
  position: relative;
  height: fit-content;
width: fit-content;
  box-shadow: 5px 12px;
    font-size: x-large;
     background-color: #ffffff;
}

.skins-section {
  background-color: var(--accent);
  width: 100%;
  display: flex;

  gap: 50px;
  justify-content: center;
  align-items: center;
  padding: 80px 0 30px 0;
}

.skins-card {
  background-color: var(--surface);
  border-radius: 15px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0px 30px 30px 30px;
}

.card-logos {
  display: flex;
  gap: 30px;
  justify-content: center;
  align-items: center;
}


.card-logos div {

  display: flex;
  flex-direction: column;
  text-align: center;
  align-items: center;
  justify-content: center;
  gap: 10px;
}

.card-logos div img {
  width: 60px;
  height: 40px;
  object-fit: contain;
}
</style>