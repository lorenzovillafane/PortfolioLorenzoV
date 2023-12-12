<template>
  <div class="container">
    <p>HOLA, SOY </p>
    <section class="animation">
      <div class="first"><div>Lorenzo Villafañe</div></div>
      <div class="second"><div>Front-End Developer</div></div>
      <div class="third"><div>Game Developer</div></div>
    </section>
  </div>
  <div class="menu-wrap">
    <input type="checkbox" class="toggler" />
    <div class="hamburger"><div></div></div>
    <div class="menu">
      <div>
        <div>
          <ul>
            <li>
              <router-link to="/About">SOBRE MI</router-link>
            </li>
            <li>
              <router-link to="/Skills">SKILLS</router-link>
            </li>
            <li>
              <router-link to="/Projects">PROJECTS</router-link>
            </li>
            <li>
              <router-link to="/Contact">CONTACT</router-link>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>
<style scoped>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
.menu-wrap {
  position: fixed;
  top: 5%;
  left: 43%;
  z-index: 1;
  background-color: green;
}
.menu-wrap .toggler {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 2;
  cursor: pointer;
  width: 50px;
  height: 50px;
  opacity: 0;
}
.menu-wrap .hamburger {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1;
  width: 60px;
  height: 60px;
  padding: 1rem;
  background: #776b5d;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
}
/*Hamburger line*/
.menu-wrap .hamburger > div {
  position: relative;
  width: 100%;
  height: 2px;
  background-color: #ebe3d5;
  display: flex;
  align-items: center;
  justify-content: center;
  transition: all 0.4s ease;
}
/*Top and bottom lines*/
.menu-wrap .hamburger > div:before,
.menu-wrap .hamburger > div:after {
  content: "";
  position: absolute;
  z-index: 1;
  top: -10px;
  width: 100%;
  height: 2px;
  background: inherit;
}
/*Moves line down*/
.menu-wrap .hamburger > div:after {
  top: 10px;
}

.menu-wrap .menu {
  position: fixed;
  top: 10px;
  left: 0;
  width: 100%;
  height: 100%;
  visibility: hidden;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
}
.menu-wrap .menu > div {
  background: #ada597;
  border-radius: 50%;
  width: 200vw;
  height: 200vw;
  display: flex;
  flex: none;
  align-items: center;
  justify-content: center;
  transform: scale(0);
  transition: all 0.4s ease;
}

.menu-wrap .menu > div > div {
  text-align: center;
  max-width: 90vw;
  max-height: 100vh;
  opacity: 0;
  transition: opacity 0.4s ease;
}
.menu-wrap .menu > div > div > ul > li {
  list-style: none;
  color: #3a332c;
  font-size: 1.5rem;
  padding: 1rem;
}
.menu-wrap .menu > div > div > ul > li > a {
  color: inherit;
  text-decoration: none;
  transition: color 0.4s ease;
}
.menu-wrap .toggler:checked ~ .menu {
  visibility: visible;
}
.menu-wrap .toggler:checked ~ .menu > div {
  transform: scale(1);
  transition-duration: 0.75s;
}
.menu-wrap .toggler:checked ~ .menu > div > div {
  opacity: 1;
  transition: opacity 0.4s ease;
}

/*MENU*/

.container {
  color: #3a332c;
  font-size: 30px;
  text-transform: uppercase;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  font-weight: bold;
  margin-top: 100%;
}
.first,
.second,
.third {
  flex: 1;
  font-size: 20px;
  text-align: center;
}
.animation {
  height: 30px;
  overflow: hidden;
  margin-left: 1rem;
}

.animation > div > div {
  padding: 0.25rem 0.75rem;
  height: 55px;
  margin-bottom: 40px;
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

@media (min-width: 500px) {
  .container {
    font-size: 40px;

    margin-top: 50%;
  }
  .first,
  .second,
  .third {
    flex: 1;
    font-size: 30px;
  }
  .animation {
    height: 35px;
  }

  .animation > div > div {
    height: 55px;
    margin-bottom: 40px;
  }
}
@media (max-width: 499px) {
  .container {
    font-size: 40px;

    margin-top: 60%;
  }
  .first,
  .second,
  .third {
    flex: 1;
    font-size: 25px;
  }
  .animation {
    height: 30px;
  }

  .animation > div > div {
    height: 55px;
    margin-bottom: 40px;
  }

  .menu-wrap {
    position: fixed;
    top: 5%;
    left: 42%;
    z-index: 1;
    background-color: green;
  }
}

@media (max-width: 365px) {
  .container {
    font-size: 25px;

    margin-top: 60%;
  }
  .first,
  .second,
  .third {
    flex: 1;
    font-size: 18px;
  }
}
@media (max-width: 278px) {
  .container {
    font-size: 20px;

    margin-top: 60%;
  }
  .first,
  .second,
  .third {
    flex: 1;
    font-size: 12px;
  }
}
@media (max-width: 212px) {
  .container {
    font-size: 15px;

    margin-top: 60%;
  }
  .first,
  .second,
  .third {
    flex: 1;
    font-size: 12px;
  }
}
</style>
<script>
export default {
  name: "MenuMobile",
};
</script>
