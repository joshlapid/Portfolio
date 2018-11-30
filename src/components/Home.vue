<template>
  <div class="wrapper">
    <router-link v-bind:to="'/about'">
      <section id="about">
        <div>
          JOSH
        </div>
      </section>
    </router-link>

    <section class="right-boxes">
      <router-link v-bind:to="'/work'">
        <div id="work">
          test
        </div>
      </router-link>
      <router-link v-bind:to="'/contact'">
        <div id="contact">
          test
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
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.wrapper {
  display: flex;
}

.right-boxes {
  width: 50vw;
  height: 100vh;
}

.right-boxes div {
  height: 50vh;
}

#about {
  width: 50vw;
  height: 100vh;
  background-image: url('../assets/headshot.jpg');
  background-position: center;
  background-size: cover;

  div {
    font-size: 35px;
  }
}

#work {
  background-image: url('../assets/back3.jpg');
  background-position: center;
  background-size: cover;
}

#contact {
  background-image: url('../assets/back5.jpg');
  background-position: center;
  background-size: cover;
}

</style>
