<template>
  <header>
    <router-link to="/">MENU</router-link>
  </header>
  <main>
    <div class="tabs">
      <input class="input" name="tabs" type="radio" id="tab-1" checked="true" />
      <label class="label" for="tab-1">HARD SKILLS</label>
      <div class="panel">
        <h1>HARD SKILLS</h1>
        <div class="hardSkills">
          <div class="code">
            <div class="estructura">
              <img src="../assets/icon/skills/vue.png" alt="" />
              <img src="../assets/icon/skills/react.png" alt="" />
              <img src="../assets/icon/skills/angular.png" alt="" />
              <img src="../assets/icon/skills/node.png" alt="" />
              <img src="../assets/icon/skills/vite.png" alt="" />
            </div>
            <div class="estilo">
              <img src="../assets/icon/skills/tailwind.png" alt="" />
              <img src="../assets/icon/skills/sass.png" alt="" />
              <img src="../assets/icon/skills/bootstrap.png" alt="" />
            </div>
            <div class="codigo">
              <img src="../assets/icon/skills/javascript.png" alt="" />
              <img src="../assets/icon/skills/java.png" alt="" />
              <img src="../assets/icon/skills/csharp.png" alt="" />
            </div>
          </div>

          <div class="design">
            <img src="../assets/icon/skills/figma.png" alt="" />
            <img src="../assets/icon/skills/adobexd.png" alt="" />
            <img src="../assets/icon/skills/photoshop.png" alt="" />
          </div>

          <div class="engine">
            <img src="../assets/icon/skills/visualcode.png" alt="" />
            <img src="../assets/icon/skills/unity.png" alt="" />
            <img src="../assets/icon/skills/godot.png" alt="" />
          </div>
        </div>
      </div>
      <input class="input" name="tabs" type="radio" id="tab-2" />
      <label class="label" for="tab-2">SOFT SKILLS</label>
      <div class="panel dos">
        <h1>SOFT SKILLS</h1>
        <div class="softSkills">
          <ul>
            <li>Adaptabilidad</li>
            <li>Trabajo en equipo</li>
            <li>resolución de problemas</li>
            <li>Creatividad</li>
            <li>Aptitudes para la resolución de conflictos</li>
            <li>Aprendizaje continuo</li>
            <li>Resiliencia</li>
            <li>Ética profesional</li>
            <li>Empatía</li>
            <li>Pensamiento crítico</li>
          </ul>
        </div>
      </div>
    </div>
  </main>
</template>
<style scoped lang="scss">
@import "../styles/skills.scss";
</style>
<script></script>
