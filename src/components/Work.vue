<template>
	<div class="page">
  	<div class="container">
  		<span class="back-icon"><router-link v-bind:to="'/'" class="home-link"><i class="fas fa-chevron-circle-left"></i></router-link></span>
	    <h1>Recent Work</h1>
	  	<div class="recent-work">
	  		<div class="item" v-for="project in projects">
	  			<h2>{{ project.name }}</h2>
	  			<a v-bind:href="project.url" target="_blank"><img v-bind:src="project.image" width="250"></a>
	  		</div>
	  	</div>
	</div>
  </div>
</template>

<script>
export default {
  name: 'work',
  data () {
  return {
    projects: [
    	{ name: 'Atlanta Pet Fair', url: 'https://atlantapetfair.org/', image: require('../assets/apfc.jpg')},
    	{ name: 'Corrao Group', url: 'http://corraogroup.com/', image: require('../assets/corrao.jpg')},
    	{ name: 'Craft Beverage Expo', url: 'https://www.craftbeverageexpo.com/', image: require('../assets/craft.jpg')},
    	{ name: 'Pokemon Index', url: 'https://herokupoke.herokuapp.com/search/all', image: require('../assets/pokemon.png')}
    ]
  }
}
}
</script>
<!-- styling for the component -->
<style lang="scss" scoped>
	.page {
		background: #333333;
		color: #ffffff;
		height: 100%;
		min-height: 100vh;

		a {
			color: #ffffff;
			font-weight: bold;
		}
	}

	.back-icon {
		font-size: 1.5em;
		position: absolute;
		right: 30px;
		top: 30px;

		.home-link {
			color: #ffffff;
		}
	}

	.container {
		padding: 40px;
		text-align: left;
	}

	.recent-work {
		display: flex;
		justify-content: space-around;
		flex-wrap: wrap;

		.item {
			text-align: center;
			margin: 10px;
		}
	}

</style>