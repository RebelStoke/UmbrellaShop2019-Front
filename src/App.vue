<template>
  <div id="app">
  <header>
    <div class="nav_container">
      <div class="leftSide">
        <div class="logo">
          DROP.
        </div>
        <div class="nav_wrapper">
          <div class="socials"><router-link to="/about" class="routerLink"><i class="fas fa-shopping-cart"/></router-link></div>
          <div class="socials"><router-link to="/" class="routerLink"><i class="fas fa-home"/></router-link></div>
        </div>
      </div>
      <div class="icons">
        <img src="./assets/logowithoutbackg.png" width="75" height="103.5">
        <div class="socials_container">
          <div class="socials"><i class="fab fa-instagram"></i></div>
          <div class="socials"><i class="fab fa-facebook"></i></div>
          <div class="socials"><i class="fab fa-youtube"></i></div>
        </div>

      </div>
    </div>
  </header>

  <main>
  <div>
  <router-view/>
  </div>
  </main>

  <footer>

  </footer>
  </div>
 <!-- <div class="design"  id="app">
    <div class="header">
      <h1 class="header1">DROP.</h1>
      <div id="icon">
        <font-awesome-icon :icon="['fas', 'user-secret']"/>
      </div>

    </div>
    <div class="logo">
      <img src="./assets/logowithoutbackg.png" width="75" height="103.5">
    </div>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
  -->
</template>

<script>
  export default {
    name: 'home',
    data() {
      return {

      }
    },
    }


</script>

<style lang="scss">
  @font-face {
    font-family: myFirstFont;
    src: url('./assets/fonts/ChunkFive-Regular.otf');
  }

  .routerLink{
    color: white;
  }
  body, html{
    padding: 0;
    margin: 0;
    background-image: url("./assets/backgroundblack.jpg");
    background-size: cover;
  }
  .invert{
    filter: invert(100%);
  }

  .nav_container{
    height: 110px;
    width: 100%;
    display: flex;
  }
  .leftSide{
    width: 50%;
    height: 108px;
    font-size: 50px;
    background: black;
    font-family: myFirstFont;
    color: white;
    display: flex;
    align-items: center;
    padding: 0px 10px 0px 20px;
    border: white solid;
    border-width: 0px 0px 2px 0px;
    justify-content: space-between;
  }
  .logo{
    display: flex;
    align-items: center;
  }
  .icons{
    width: 50%;
    display: flex;
    justify-content: flex-end;
    font-size: 40px;
    color: black;
    background-color: white;
    border: black solid;
    border-width: 0px 0px 2px 0px;

  }
.nav_wrapper{
  width:150px;
  height: 100px;
  font-size: 40px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}

.socials:hover{
  -webkit-transform: scale(1.3);
  -ms-transform: scale(1.3);
  transform: scale(1.3);
}
  .socials_container{
    width: 200px;
    height: 100px;
    display: flex;
    justify-content: space-around;
    align-items: center;;
  }

</style>
