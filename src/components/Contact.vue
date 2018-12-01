<template>
	<div class="page">
  	<div class="container">
  		<span class="back-icon"><router-link v-bind:to="'/'" class="home-link"><i class="fas fa-chevron-circle-left"></i></router-link></span>
	    <h1>Get In Touch</h1>
	  	<p>Please contact me and send me your questions and inquiries.</p>
	  	<p><a href="mailto:lapidjoshua@gmail.com" target="_top">lapidjoshua@gmail.com</a> | 619.623.1598 | San Diego, California</p>
	</div>
  </div>
</template>

<script>
export default {
  name: 'contact'
}
</script>
<!-- styling for the component -->
<style lang="scss" scoped>
	.page {
		background: #000000;
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

</style>