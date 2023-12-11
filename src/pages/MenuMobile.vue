
<template><div class="menu-wrap">
    <input type="checkbox" class="toggler">   
    <div class="hamburger"><div></div></div>  
    <div class="menu">   
    <div>
      <div>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </div>
      </div>
    </div>
  </div>
</template>  
<style scoped >
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
.menu-wrap {
  position: fixed;
  top: 0%;
  left: 48.5%;
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
  background: red;
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
  background-color: #fff;
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
.menu-wrap .menu > div{
  background: skyblue;
  border-radius: 50%;
  width: 200vw;
  height: 200vw;
  display:flex;
  flex: none;
  align-items: center;
  justify-content: center;
  transform: scale(0);
  transition: all .4s ease;
}

.menu-wrap .menu > div > div{
  text-align: center;
  max-width: 90vw;
  max-height: 100vh;
  opacity: 0;
  transition: opacity .4s ease;
}
.menu-wrap .menu > div > div > ul > li{
  list-style: none;
  color: black;
  font-size: 1.5rem;
  padding: 1rem;
}
.menu-wrap .menu > div > div > ul > li > a{
  color: inherit;
  text-decoration: none;
  transition: color .4s ease;
}
.menu-wrap .toggler:checked ~ .menu{
  visibility: visible;
}
.menu-wrap .toggler:checked ~ .menu > div{
  transform: scale(1);
  transition-duration: .75s;
}
.menu-wrap .toggler:checked ~ .menu > div > div{
  opacity: 1;
  transition: opacity .4s ease;
}

</style>
<script></script>