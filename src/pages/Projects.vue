<template>
    <header>
    <div class="back">
      <router-link to="/">MENU</router-link>
    </div >
    <div class="menu"> 
      <router-link to="/About">SOBRE MI</router-link>
      <router-link to="/Skills">SKILLS</router-link>
        <router-link to="/Contact">CONTACTO</router-link>
       
    </div>
  </header>
  <main>
    <div class="tabs">
      <input class="input" name="tabs" type="radio" id="tab-1" checked="true" />
      <label class="label" for="tab-1">PROFESSOR SLOWBRO</label>
      <div class="panel">
        <a href="https://professor-slowbro.vercel.app/" target="_blank"><h1>PROFESSOR SLOWBRO</h1></a>
        <p>
          Professor Slowbro es una web dedicada a Pokémon y su ecosistema
          competitivo.
        </p>
        <div class="descripcionProfessor">
          <img
            src="../assets/projects/professorslowbro.png"
            alt="professorSlowbro"
          />
        </div>
      </div>

      <input class="input" name="tabs" type="radio" id="tab-3" />
      <label class="label" for="tab-3">TASKAPP</label>
      <div class="panel tres">
          <a href="https://task-app2-taupe.vercel.app/" target="_blank"><h1>TASKAPP</h1> </a>
        <p>
          Taskapp es una aplicacion para registrar tus tareas y llevar un
          registro de ellas.
        </p>
        <div class="descripcionTaskapp">
          <img src="../assets/projects/taskapp.png" alt="taskapp" />
        </div>
      </div>
    </div>
  </main>
</template>
<style scoped lang="scss">
@import "../styles/projects.scss";
</style>
<script></script>
