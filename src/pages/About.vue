<template>
  <header>
    <div class="back">
      <router-link to="/">MENU</router-link>
    </div >
    <div class="menu"> 
     
      <router-link to="/Skills">SKILLS</router-link>
        <router-link to="/Projects">PROYECTOS</router-link>
        <router-link to="/Contact">CONTACTO</router-link>
       
    </div>
  </header>
  <main>
    <div class="tabs">
      <input class="input" name="tabs" type="radio" id="tab-1" checked="true" />
      <label class="label" for="tab-1">SOBRE MI</label>
      <div class="panel">
        <h1>SOBRE MI</h1>
        <p>
          Hola soy Lorenzo, tengo 24 años y actualmente estoy viviendo en
          Argentina (Mendoza). Soy desarrollador Frontend JR y en mis tiempos
          libres desarollador de videojuegos indies. Mi enfoque principal está
          en la creación de experiencias visuales impactantes y funcionales en
          la web. Busco oportunidades para adentrarme en el mundo laboral y
          aplicar mis habilidades. Siempre estoy dispuesto a aprender y aportar
          nuevas ideas a proyectos innovadores.
        </p>
        
       
        <div class="containerSection">
          <img
            src="../assets/imagen/yo.jpg"
            alt="LorenzoVillafañe"
            id="profileImg"
          />
        </div><div class="curriculum">
           <a href="../assets/Lorenzo Villafañe CV.pdf" download ><img src="../assets/icon/about/cv.png" alt="cv">
          Descargar CV
          
        </a>
        </div>
      </div>
      <input class="input" name="tabs" type="radio" id="tab-2" />
      <label class="label" for="tab-2">ESTUDIOS</label>
      <div class="panel dos">
        <h1>ESTUDIOS</h1>
        <ul>
          <li>
            Desarrollador Web Frontend VueJS | MINDHUB - ArgentinaPrograma
          </li>
          <li>
            Desarrollador Web Frontend ReactJS | Universidad Tecnológica
            Nacional
          </li>
          <li>Digital Skills: User Experience | Accenture</li>
          <li>
            Estudiante de Ingenieria en Sistemas | Universidad Tecnológica
            Nacional FRM
          </li>
        </ul>
      </div>
      <input class="input" name="tabs" type="radio" id="tab-3" />
      <label class="label" for="tab-3">HOBBIES</label>
      <div class="panel tres">
        <h1>HOBBIES</h1>
        <div class="hobbiesImg">
          <img src="../assets/icon/about/futbol.png" alt="futbol" />
          <img src="../assets/icon/about/montaña.png" alt="montaña" />
          <img src="../assets/icon/about/wine.png" alt="vino" />
          <img src="../assets/icon/about/icons8-pokemon-48.png" alt="pokémon" />
          <img
            src="../assets/icon/about/icons8-escuchar-musica-en-auriculares-48.png"
            alt="musica"
          />
          <img
            src="../assets/icon/about/icons8-argentina-48.png"
            alt="Argentina"
          />
          <img src="../assets/icon/about/gameboy.png" alt="Videojuegos" />
        </div>
      </div>
    </div>
  </main>
</template>
<style scoped lang="scss">
@import "../styles/about.scss";
</style>
