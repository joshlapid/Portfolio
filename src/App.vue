<template>
  <div id="app">
    <transition name="page-animation">
      <router-view/>
    </transition>
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

  .page {
    position: fixed;
    width: 100%;
  }

  .page-animation-enter-active {
    animation: coming 0.5s;
    /*animation-delay: 0.5s;*/
    opacity: 0;
  }

  .page-animation-leave-active {
    animation: going 0.5s;
  }

    @keyframes coming {
      from {
      }

      to {
        opacity: 1;
      }
    }


  @keyframes going {
    from {
    }

    to {
      opacity: 0;
    }
  }

  @media only screen and (max-width: 600px) {
    h1 {
      font-size: 2em;
    }
  }
</style>
