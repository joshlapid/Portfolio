<template>
  <div class="page">
  	<div class="container">
  		<span class="back-icon"><router-link v-bind:to="'/'" class="home-link"><i class="fas fa-chevron-circle-left"></i></router-link></span>
	    <h1>A Little About Me</h1>
	  	<p>I am a front-end web developer with experience in a marketing environment. I started tinkering with programming in my spare time, and discovered that it fed my appetite for creativity. When my appreciation for coding grew, I enrolled in a full-stack web development bootcamp. I am passionate in creating functional yet aesthetic websites.</p>
	  	<h1>My Skills</h1>
	  	<div class="skills-icons">
	  		<p>
	  			<i class="devicon-css3-plain-wordmark skills_icon"></i>
			    <i class="devicon-html5-plain-wordmark skills_icon"></i>
			    <i class="devicon-javascript-plain skills_icon"></i>
			    <i class="devicon-vuejs-plain-wordmark"></i>
			    <i class="devicon-sass-original skills_icon"></i>
			    <i class="devicon-bootstrap-plain-wordmark skills_icon"></i>
			    <i class="devicon-wordpress-plain"></i>
			    <i class="devicon-php-plain skills_icon"></i>
			    <i class="devicon-jquery-plain-wordmark skills_icon"></i>
			</p>
		</div>
	</div>
  </div>
</template>

<script>
export default {
  name: 'about'
}
</script>
<!-- styling for the component -->
<style lang="scss" scoped>
	.page {
		position: static;
		background: #144057;
		color: #ffffff;
		height: 100%;
		min-height: 100vh;
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

	.skills-icons i {
		font-size: 4em;
		line-height: 1.2em;
		margin: 0px 10px;
	}
</style>