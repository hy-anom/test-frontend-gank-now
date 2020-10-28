<template>
	<section class="hero">
		<h1 class="hero-title">
			The best of your <span>gaming moments,</span><br>
			All in one page.
		</h1>
		<div class="hero-splash"></div>
	</section>
</template>

<script>
export default {

  name: 'Hero',

  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.hero {
	background-image: linear-gradient(transparent, #393E5E);
	padding: 70px 20px 0;
	height: 540px;
	position: relative;
	margin-bottom: 120px;

	@media (max-width: 640px) {
		height: 420px;
	}
}

.hero-title {
	text-align: center;
	font-weight: bold;
	font-size: 24px;
	span {
		color: #ED5C5E;
	}
}

.hero-splash {
	background-image: url('../assets/img-laptop.png');
	background-size: contain;
	background-position: center;
	background-repeat: no-repeat;
	height: 540px;
	max-width: 800px;
	margin: auto;

	@media (max-width: 640px) {
		height: 420px;
	}
}
</style>