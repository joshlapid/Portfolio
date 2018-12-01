<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  body {
    margin: 0px;
    font-size: 20px;
  }

  h1 {
    font-size: 3em;
    margin-bottom: .3em;
  }

  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  @media only screen and (max-width: 600px) {
    h1 {
      font-size: 2em;
    }
  }
</style>
