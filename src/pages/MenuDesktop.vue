<template>
  <main>
    <div class="container">
      <p>HOLA, SOY </p>
      <section class="animation">
        <div class="first"><div>Lorenzo Villafañe</div></div>
        <div class="second"><div>Front-End Developer</div></div>
        <div class="third"><div>Game Developer</div></div>
      </section>
    </div>
    <span><span></span></span>
    <div class="wrap">
      <router-link to="/Skills"
        ><div>
          <img
            src="../assets/imagen/icons8-programación-96.png"
            alt="skills"
          />SKILLS
        </div></router-link
      >
      <router-link to="/Projects"
        ><div>
          <img
            src="../assets/imagen/icons8-documentos-de-producto-96.png"
            alt="proyectos"
          />PROYECTOS
        </div></router-link
      >
      <router-link to="/Contact"
        ><div>
          CONTACTO<img
            src="../assets/imagen/icons8-buzón-con-carta-96.png"
            alt="contacto"
          /></div
      ></router-link>
      <router-link to="/About"
        ><div>
          SOBRE MI<img
            src="../assets/imagen/icons8-cuenta-de-prueba-96.png"
            alt="sobremi"
          /></div
      ></router-link>
    </div>
  </main>
</template>
<style scoped lang="scss">
body,
html {
  margin: 0;
  padding: 0;
  height: 100%;
  background-color: #243a73;
}
body {
  background: #243a73;
  box-shadow: inset 0 0 20vmin 0 #585247;
}
.wrap {
  position: relative;
  width: 40vmin;
  height: 40vmin;
  margin: 0 auto;
  background: inherit;
  transform: scale(0.2) translatez(0px);
  opacity: 0;
  transition: transform 0.5s, opacity 0.5s;
}
a {
  position: absolute;
  left: 0;
  top: 0;
  width: 47.5%;
  height: 47.5%;
  overflow: hidden;
  transform: scale(0.5) translateZ(0px);
  background: #f2ebe9;
}
a div {
  height: 100%;
  background-size: cover;
  opacity: 0.5;
  transition: opacity 0.5s;
  border-radius: inherit;
}
a:nth-child(1) {
  border-radius: 40vmin 0 0 0;
  transform-origin: 110% 110%;
  transition: transform 0.4s 0.15s;
  text-decoration: none;
  font-weight: bold;
}
a:nth-child(1) div {
  background-color: #BBAB8C;
  background-size: 360px;
  font-size: 25px;
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  flex-direction: column;
  text-decoration: none;
  font-size: bold;
  color: #3a332c;
}
a:nth-child(2) {
  border-radius: 0 40vmin 0 0;
  left: 52.5%;
  font-weight: bold;
  transform-origin: -10% 110%;
  transition: transform 0.4s 0.2s;
  text-decoration: none;
}
a:nth-child(2) div {
  background-color: #BBAB8C;
  background-size: 360px;
  font-size: 25px;
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  flex-direction: column;
  text-decoration: none;
  font-size: bold;
  color: #3a332c;
}
a:nth-child(3) {
  border-radius: 0 0 0 40vmin;
  top: 52.5%;
  transform-origin: 110% -10%;
  font-weight: bold;
  text-decoration: none;
  transition: transform 0.4s 0.25s;
}
a:nth-child(3) div {
  background-color: #BBAB8C;
  background-size: 360px;
  font-size: 25px;
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  flex-direction: column;
  text-decoration: none;
  font-size: bold;
  color: #3a332c;
}
a:nth-child(4) {
  border-radius: 0 0 40vmin 0;
  top: 52.5%;
  left: 52.5%;
  text-decoration: none;
  font-weight: bold;
  transform-origin: -10% -10%;
  transition: transform 0.4s 0.3s;
}
a:nth-child(4) div {
  background-color: #BBAB8C;
  background-size: 360px;
  font-size: 25px;
  display: flex;
  justify-content: center;
  align-items: center;
  align-content: center;
  flex-direction: column;
  text-decoration: none;
  font-size: bold;
  color:#3a332c;
}
a:nth-child(4) div img {
  width: 84px;
}

span {
  position: relative;
  display: block;
  margin: 0 auto;
  top: 25vmin;
  width: 10vmin;
  height: 10vmin;
  border-radius: 100%;
  background: #776b5d;
  transform: translateZ(0px);
}
span span {
  position: absolute;
  width: 60%;
  height: 3px;
  background: #f2ebe9;

  left: 20%;
  top: 50%;
  border-radius: 0;
}
span span:after,
span span:before {
  content: "";
  position: absolute;
  left: 0;
  top: -1.5vmin;
  width: 100%;
  height: 100%;
  background: inherit;
}
span span:after {
  top: 1.5vmin;
}
span:hover + .wrap,
.wrap:hover {
  transform: scale(0.8) translateZ(0px);
  opacity: 1;
}
span:hover + .wrap a,
.wrap:hover a {
  transform: scale(1) translatez(0px);
}
a:hover div {
  opacity: 1;
  transform: translatez(0px);
}

/*ESTILO H1 */

.container {
  color: #3a332c;
  font-size: 60px;
  text-transform: uppercase;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  font-weight: bold;
  margin-top: 15%;
}
.animation {
  height: 80px;
  overflow: hidden;
  margin-left: 1rem;
}

.animation > div > div {
  padding: 0.25rem 0.75rem;
  height: 60px;
  margin-bottom: 30px;
  display: inline-block;
}

.animation div:first-child {
  animation: text-animation 8s infinite;
}

.first div {
  color: #ebe3d5;
  background-color: #5699ff;
}
.second div {
  color: #ebe3d5;
  background-color: #ffc800;
}
.third div {
  color: #ebe3d5;
  background-color: #fc2a2a;
}

@keyframes text-animation {
  0% {
    margin-top: 0;
  }
  10% {
    margin-top: 0;
  }
  20% {
    margin-top: -5.62rem;
  }
  30% {
    margin-top: -5.62rem;
  }
  40% {
    margin-top: -11.24rem;
  }
  60% {
    margin-top: -11.24rem;
  }
  70% {
    margin-top: -5.62rem;
  }
  80% {
    margin-top: -5.62rem;
  }
  90% {
    margin-top: 0;
  }
  100% {
    margin-top: 0;
  }
}

@media (max-width: 1450px) {
  .container {
    color: #3a332c;

    text-transform: uppercase;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    flex-direction: column;
    font-weight: bold;
  }
  .first,
  .second,
  .third {
    flex: 1;
    text-align: center;
  }
  .animation {
    overflow: hidden;
    margin-left: 1rem;
  }

  .animation > div > div {
    padding: 0.25rem 0.75rem;

    margin-bottom: 30px;
    display: inline-block;
  }
}

@media (max-width: 1100px) {
  .container {
    color: #3a332c;
    font-size: 50px;
    text-transform: uppercase;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    font-weight: bold;
  }
  .first,
  .second,
  .third {
    flex: 1;
    text-align: center;
  }
  .animation {
    height: 60px;
    overflow: hidden;
    margin-left: 1rem;
  }

  .animation > div > div {
    padding: 0.25rem 0.75rem;
    height: 60px;
    margin-bottom: 30px;
    display: inline-block;
  }
}
</style>
<script>
export default {
  name: "MenuDesktop",
};
</script>
