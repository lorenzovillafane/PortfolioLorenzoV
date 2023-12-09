<template>
  <header>
    <router-link to="/">BACK TO MENU</router-link>
  </header>
  <main>
    <div class="tabs">
      <input class="input" name="tabs" type="radio" id="tab-1" checked="true" />
      <label class="label" for="tab-1">PROFESSOR SLOWBRO</label>
      <div class="panel">
        <h1>PROFESSOR SLOWBRO</h1>
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
        <h1>TASKAPP</h1>
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
