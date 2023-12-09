<template>
    <header>
      <router-link to="/">BACK TO MENU</router-link>
    </header>
    <main>
    <div class="tabs">
      <input class="input" name="tabs" type="radio" id="tab-1" checked="true" />
      <label class="label" for="tab-1">CONTACT</label>
      <div class="panel">
        <h1></h1>
    
<form id="form" class="topBefore">
		
        <input id="name" type="text" placeholder="NAME">
        <input id="email" type="email" placeholder="E-MAIL">
        <textarea id="message" type="text" placeholder="MESSAGE"></textarea>
<input id="submit" type="submit" value="GO!">

</form>
      </div>
      <input class="input" name="tabs" type="radio" id="tab-2" />
      <label class="label" for="tab-2">SOCIAL</label>
      <div class="panel dos">
        <a href=""><img src="../assets/icon/social/linkedin.png" alt="linkedin"></a>
        <a href=""><img src="../assets/icon/social/telegram.png" alt="telegram"></a>
        <a href=""><img src="../assets/icon/social/whatsapp.png" alt="wpp"></a>
        <a href=""><img src="../assets/icon/social/github.png" alt="github"></a>
        <a href=""><img src="../assets/icon/social/gmail.png" alt="gmail"></a>
      </div>
    </div>
  </main>
    
    </template>
<style scoped lang="scss">
@import "../styles/contact.scss";
</style>
<script></script>