<template>
  <header>
    <nav role="navigation" class="primary-navigation">
  <ul>
    <li><router-link to="/About">SOBRE MI</router-link></li>
    <li><router-link to="/Skills">SKILLS</router-link></li>
    <li><router-link to="/Projects">PROYECTOS</router-link></li>
    <li><router-link to="/Contact">CONTACTO</router-link></li>
    <li><p></p></li>
  </ul>
</nav>
  </header>
  <main>
    <div class="container">
      <p>HOLA, SOY </p>
      <section class="animation">
        <div class="first"><div>Lorenzo Villafañe</div></div>
        <div class="second"><div>Front-End Developer</div></div>
        <div class="third"><div>Game Developer</div></div>
      </section>
    </div>
  </main>
</template>
<style scoped lang="scss">
/*NAVBAR*/
nav {
  &.primary-navigation {
    margin: 0 auto;
    display: block;
  
    padding: 20px;  
    text-align: center;
    font-size: 20px;
    ul li p{
      list-style: none;
      margin: 0 auto;
      border-left: 2px solid #B0A695;
      display: inline-block;
  
      position: relative;
      text-decoration: none;
      text-align: center;
      font-family: arvo;

    }

    ul li {
      list-style: none;
      margin: 0 auto;
      border-left: 2px solid #B0A695;
      display: inline-block;
      padding: 0 30px;
      position: relative;
      text-decoration: none;
      text-align: center;
      font-family: arvo;
    }

    li a {
      color: #3a332c;
    }

    li a:hover {
      color: #776B5D;
    }

    li:hover {
      cursor: pointer;
    }

    ul li:hover > ul,
    ul li ul:hover {
      visibility: visible;
      opacity: 1;
      display: block;
      min-width: 250px;
      text-align: left;
      padding-top: 20px;
      box-shadow: 0px 3px 5px -1px #ccc;
    }

    ul li ul li {
      clear: both;
      width: 100%;
      text-align: left;
      margin-bottom: 20px;
      border-style: none;
    }

    ul li ul li a:hover {
      padding-left: 10px;
      border-left: 2px solid #3a332c;
      transition: all 0.3s ease;
    }
  }
}

a {

    text-decoration: none;

    &:hover {
        color: #3CA0E7;
    }
 
}

 ul li ul li a { transition: all 0.5s ease; }



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
