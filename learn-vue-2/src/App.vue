<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/Vader">Väder</router-link>
      <router-link to="/Social">Social</router-link>
      <router-link to="/Calender">Kalender</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="scss">

* {
  margin:0;
}
body {
  margin:0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  margin: 0;
  padding: 1.25em;
  background-color: #00A6C4;
  text-align:left;
  position: fixed;
  width: 100vw;
  a {
    font-size: 1.5em;
    font-weight: bold;
    color: #fff;
    text-decoration: none;
    margin-right: 0.5em;
    &.router-link-exact-active {
      text-decoration: underline;
    }
  }
}

</style>
