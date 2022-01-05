<template>
  <b-container fluid id="app">
    <b-row align-h="around" class="nav" align-v="center">
      <b-col xl="4" class="left-section">
        <div class="nav-logo">
          <b-img :src="require('./assets/logo-dummy.png')" fluid-grow alt="logo-dummy"></b-img>
        </div>
      </b-col>
      <b-col xl="4" class="right-section">
       <b-link href="/">Home</b-link>
       <b-link href="/about">Favorites</b-link>
      </b-col>
    </b-row>
    <router-view></router-view>
    <b-row class="footer">
      <b-col>&copy; copyriright</b-col>
    </b-row>
  </b-container>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
#app {
  font-family: Popins, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #00BFFF;
}

.nav {
  height: 60px;
}

/* //ToDo fix this  */
.nav-logo {
  height: 80%;
}

.nav img {
  width: 100%;
  height: 100%;
}

a {
  text-decoration: none !important;
  color: white !important;
  margin: 15px;
  font-size: 1.5em;
  padding-bottom: 4px;
}

a:hover {
  border-bottom: 1.7px solid rgba(255, 255, 255, 0.7);
}
.left-section div {
  width: 20%;
  height: 30px;
  background-color: white;
}

.right-section {
  text-align: right;
}



</style>
