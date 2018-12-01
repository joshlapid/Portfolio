<template>
  <div class="wrapper">

    <router-link v-bind:to="'/about'" class="home-link">
      <section id="about">
        <h1 class="section-header">
          {{ headline1 }}
        </h1>
      </section>
    </router-link>

    <section class="right-boxes">
      <router-link v-bind:to="'/work'" class="home-link">
        <div id="work">
          <h1 class="section-header">
            <span>{{ headline2 }}</span>
          </h1>
        </div>
      </router-link>
      <router-link v-bind:to="'/contact'" class="home-link">
        <div id="contact">
          <h1 class="section-header">
            {{ headline3 }}
          </h1>
        </div>
      </router-link>
    </section>

  </div>
</template>

<script>
  export default {
    name: 'Home',
    data () {
      return {
        headline1: 'JOSH',
        headline2: 'WORK',
        headline3: 'CONTACT'
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
  .home-link {
    text-decoration: none;
    color: #ffffff;
    font-weight: bold;
  }

  .wrapper {
    display: flex;
  }

  .section-header {
    text-shadow: 0px 0px 3px #000000;
  }

  #about {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50vw;
    height: 100vh;
    background-image: url('../assets/headshot.jpg');
    background-position: center;
    background-size: cover;
  }



  .right-boxes div {
    display: flex;
    width: 50vw;
    height: 50vh;
    background-position: center;
    background-size: cover;
    align-items: center;
    justify-content: center;
  }

  #work {
    background-image: url('../assets/back3.jpg');
    .section-header {
      text-decoration: none;
    }
  }

  #contact {
    background-image: url('../assets/back5.jpg');
  }

  @media only screen and (max-width: 600px) {
    .wrapper {
      display: block;
    }

    #about {
      width: 100%;
      height: 34vh;
    }

    .right-boxes div {
      width: 100%;
      height: 33vh;
    }

  }

</style>
