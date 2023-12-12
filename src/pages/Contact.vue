<template>
   <header>
    <div class="back">
      <router-link to="/">MENU</router-link>
    </div >
    <div class="menu"> 
      <router-link to="/About">SOBRE MI</router-link>
      <router-link to="/Skills">SKILLS</router-link>
        <router-link to="/Projects">PROYECTOS</router-link>

       
    </div>
  </header>
  <main>
    <div class="tabs">
      <input class="input" name="tabs" type="radio" id="tab-1" checked="true" />
      <label class="label" for="tab-1">CONTACTO</label>
      <div class="panel">
        <h1>CONTACTO</h1>

        <form id="form" class="topBefore">
          <input id="name" type="text" placeholder="NOMBRE" />
          <input id="asunto" type="text" placeholder="ASUNTO" />
          <input id="email" type="email" placeholder="E-MAIL" />
          <textarea id="message" type="text" placeholder="MENSAJE"></textarea>
          <input id="submit" type="submit" value="ENVIAR" />
        </form>
      </div>
      <input class="input" name="tabs" type="radio" id="tab-2" />
      <label class="label" for="tab-2">SOCIAL</label>
      <div class="panel dos">
        <h1>REDES SOCIALES</h1>
        <div class="socialPanel">
          <a href="https://www.linkedin.com/in/lorenzo-villafa%C3%B1e/" target="_blank"
            ><img src="../assets/icon/social/linkedin.png" alt="linkedin"
          /></a>
          <a href="https://telegram.me/lorenvillafane" target="_blank"
            ><img src="../assets/icon/social/telegram.png" alt="telegram"
          /></a>
          <a href="https://wa.me/542613672542" target="_blank"
            ><img src="../assets/icon/social/whatsapp.png" alt="wpp"
          /></a>
          <a href="https://github.com/lorenzovillafane" target="_blank"
            ><img src="../assets/icon/social/github.png" alt="github"
          /></a>
        </div>
      </div>
    </div>
  </main>
</template>
<style scoped lang="scss">
@import "../styles/contact.scss";
</style>
<script></script>
