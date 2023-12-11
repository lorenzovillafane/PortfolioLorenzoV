<template>
  <header>
    <router-link to="/">MENU</router-link>
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
          <a href=""
            ><img src="../assets/icon/social/linkedin.png" alt="linkedin"
          /></a>
          <a href=""
            ><img src="../assets/icon/social/telegram.png" alt="telegram"
          /></a>
          <a href=""
            ><img src="../assets/icon/social/whatsapp.png" alt="wpp"
          /></a>
          <a href=""
            ><img src="../assets/icon/social/github.png" alt="github"
          /></a>
          <a href=""
            ><img src="../assets/icon/social/gmail.png" alt="gmail"
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
