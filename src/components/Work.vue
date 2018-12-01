<template>
	<div class="page">
  	<div class="container">
  		<span class="back-icon"><router-link v-bind:to="'/'" class="home-link"><i class="fas fa-chevron-circle-left"></i></router-link></span>
	    <h1>Recent Work</h1>
	  	<div class="recent-work">
	  		<div class="item">
	  			<h2>Atlanta Pet Fair</h2>
	  			<img src="../assets/apfc.jpg" width="250">
	  		</div>
	  		<div class="item">
	  			<h2>Corrao Group</h2>
	  			<img src="../assets/corrao.jpg" width="250">
	  		</div>
	  		<div class="item">
	  			<h2>Craft Beverage Expo</h2>
	  			<img src="../assets/craft.jpg" width="250">
	  		</div>
	  		<div class="item">
	  			<h2>Pokemon Index</h2>
	  			<img src="../assets/pokemon.png" width="250">
	  		</div>
	  	</div>
	</div>
  </div>
</template>

<script>
export default {
  name: 'work'
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