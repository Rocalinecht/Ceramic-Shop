<template>
  <div id="app">

    <div>
      <b-navbar variant="faded" type="light" >
        <b-navbar-brand tag="h1" class="mb-0">Ceramic Shop </b-navbar-brand>
        <b-navbar-nav class="ml-auto">
          <b-nav-item right><router-link to="/">Home </router-link> </b-nav-item>
          <b-nav-item right><router-link to="/ceramic">Ceramic</router-link> </b-nav-item>
          <b-nav-item right><router-link to="/about">About</router-link></b-nav-item>
          <b-nav-item right><router-link to="/contact">Contact</router-link> </b-nav-item>    
        </b-navbar-nav>
      </b-navbar>
    </div>
    <router-view/>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

</style>
