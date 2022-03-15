<template>
  <header>
    <nav class="container">
      <a href="/"><img alt="wdev" id="logo" src="https://raw.githubusercontent.com/william-costa/wdev-mock-site-resources/master/assets/images/wdev.svg"></a>
      <img id="menu-button" src="https://raw.githubusercontent.com/william-costa/wdev-mock-site-resources/master/assets/images/menu.svg" alt="Abrir menu">
      <div id="menu-overlay"></div>
      <div id="menu-items">
        <img alt="wdev" id="menu-logo" src="https://raw.githubusercontent.com/william-costa/wdev-mock-site-resources/master/assets/images/wdev.svg">
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/videos">Video</a></li>
          <li><a href="/sobre">Sobre</a></li>
          <li><a href="/contato">Contato</a></li>
        </ul>
      </div>
    </nav>
  </header>
</template>

<script>
import '../styles/global.css'
export default {
  name: 'Nav-bar',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
header{
  background-color: var(--color-background-nav);
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
}
nav{
  display: flex;
  justify-content: space-between;
}
.container{
  width: 90% ;
}

#logo{
  width: 130px;
}

#menu-button{
  width: 30px;
}
#menu-overlay{
  position: fixed;
  top: 0;
  left: 0;
  width: 40%;
  height: 100vh;
  background-color: #000000;
  opacity: 0.8;
}
#menu-logo{
  width: 110px;
  margin-top: 30px;
}

#menu-items{
  position: fixed;
  top: 0%;
  right: 0;
  background-color: var(--color-background-nav);
  width: 60%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
}
ul{
  list-style: none;
}
ul li{
  margin: 20px 0px;
}
ul li a{
  color: var(--color-text-light);
}
</style>
