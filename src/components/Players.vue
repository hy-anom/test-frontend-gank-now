<template>
	<section class="players">
		<div class="players-search">
			<p>
				Reserve your own free gamer profile and be the pioneers of Gank, an upcoming gaming network where your gaming career takes flight!
			</p>
			<div class="search-container">
				<search-bar></search-bar>	
			</div>
			<p>12000 gamers profile so far.</p>
		</div>

		<div class="player-slider">
			<h2 class="slider-title">Who's already on Gank?</h2>
			<slider></slider>
		</div>
	</section>
</template>

<script>
import SearchBar from './SearchBar.vue';
import Slider from './Slider.vue';

export default {
  name: 'Players',
	components: {
    SearchBar,
    Slider
  },
  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.players {
	padding: 0 20px;
	margin-bottom: 100px;
}
.players-search {
	p {
		max-width: 400px;
		text-align: center;
		margin: auto;
		font-size: 14px;
	}
}
.search-container {
	display: flex;
	justify-content: center;
	padding: 20px 0;
}

.player-slider {
	max-width: 1200px; 
	margin: auto;

	.slider-title {
		font-size: 24px;
		font-weight: bold;
		text-align: center;
		margin-top: 50px;
		margin-bottom: 40px;
	}
}
</style>