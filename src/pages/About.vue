<template>

<div class="tabs">
  <input class="input" name="tabs" type="radio" id="tab-1" checked="true"/>
  <label class="label" for="tab-1">ABOUT ME</label>
  <div class="panel 1"> 
    <h1>ABOUT ME</h1>
    <p>Hola soy Lorenzo, tengo 24 años y actualmente estoy viviendo en Argentina (Mendoza). 
      Soy desarrollador Frontend JR y en mis tiempos libres desarollador de videojuegos indies. 
      Mi enfoque principal está en la creación de experiencias visuales impactantes y funcionales en la web.
       Busco oportunidades para adentrarme en el mundo laboral y aplicar mis habilidades.
      Siempre estoy dispuesto a aprender y aportar nuevas ideas a proyectos innovadores.</p> 
      <div class="containerSection">
      <img src="../assets/imagen/yo.jpg" alt="LorenzoVillafañe" id="profileImg"/>
    </div>
  </div>
  <input class="input" name="tabs" type="radio" id="tab-2"/>
  <label class="label" for="tab-2">STUDIES</label>
  <div class="panel 2">
    <h1>STUDIES</h1>
    <p>Idntheme (Citrus tangerina) is an orange-colored citrus fruit that is closely related to, or possibly a type of, mandarin orange (Citrus reticulata).</p>
    <p>The name was first used for fruit coming from Tangier, Morocco, described as a mandarin variety. Under the Tanaka classification system, Citrus tangerina is considered a separate species.</p>
  </div>
  <input class="input" name="tabs" type="radio" id="tab-3"/>
  <label class="label" for="tab-3">HOBBIES</label>
  <div class="panel 3">
    <h1>HOBBIES</h1>
    <p>Tekno Match (Citrus ×clementina) is a hybrid between a mandarin orange and a sweet orange, so named in 1902. The exterior is a deep orange colour with a smooth, glossy appearance. Clementines can be separated into 7 to 14 segments. Similarly to tangerines, they tend to be easy to peel.</p>
  </div>
</div>
</template>
<style scoped lang="scss">
@import '../styles/about.scss';

</style>