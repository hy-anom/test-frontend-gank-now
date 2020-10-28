<template>
	<section class="icons">
		<div class="icon-splash"></div>

		<div class="icon-search">
			<p class="icon-search-title">Reserve your gamer profile now.</p>
			<div class="search-container">
				<search-bar></search-bar>	
			</div>
			<p>12000 gamer profiles reserved so far</p>
		</div>

		<div class="">
			<p class="icons-grid-title">
				And be part of an upcoming next-gen gaming network
			</p>
			<div class="icons-grid">
				<div class="icon-item">
					<div class="icon-image">
						<img src="../assets/ic-key.png">
					</div>
					<p class="icon-item-title">GAME COACHING</p>
					<p class="icon-item-caption">Find coaches or become a coach.</p>
				</div>
				<div class="icon-item">
					<div class="icon-image">
						<img src="../assets/ic-male-figure.png">
					</div>
					<p class="icon-item-title">FIND PLAYER</p>
					<p class="icon-item-caption">
						Find like-minded players to play with.
					</p>
				</div>
				<div class="icon-item">
					<div class="icon-image">
						<img src="../assets/ic-cup.png">
					</div>
					<p class="icon-item-title">ORGANIZE SCRIMS</p>
					<p class="icon-item-caption">Find teams to scrim with.</p>
				</div>
				<div class="icon-item">
					<div class="icon-image">
						<img src="../assets/ic-lightning.png">
					</div>
					<p class="icon-item-title">MERCENERIES</p>
					<p class="icon-item-caption">
						Engage gamers to help you with your quests, or be one.
					</p>
				</div>
			</div>			
		</div>
	</section>
</template>

<script>
import SearchBar from './SearchBar.vue';

export default {
  name: 'Icons',
  components: {
  	SearchBar
  },
  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.icons {
	margin-top: 60px;
}

.icon-splash {
	background-image: url('../assets/img-laptop.png');
	background-size: contain;
	background-position: center;
	background-repeat: no-repeat;
	height: 300px;
	max-width: 600px;
	margin: auto;
} 

.icon-search {
	p {
		max-width: 400px;
		text-align: center;
		margin: auto;
		font-size: 14px;
	}

	.icon-search-title {
		font-size: 24px;
	}

}
.search-container {
	display: flex;
	justify-content: center;
	padding: 20px;
}

.icons-grid {
	display: flex;
	padding: 0 20px;
	max-width: 720px;
	margin: auto;
	flex-wrap: wrap;
	justify-content: center;
}
.icons-grid-title {
	font-size: 24px;
	text-align: center;
	margin: 50px auto 30px;
	width: 300px;
}
.icon-item {
	margin: 0 20px;
	text-align: center;
	flex-grow: 1;
	flex-basis: 0;

	@media (max-width: 640px) {
		flex-basis: 40%;
	}
}
.icon-image {
	background-color: #242734;
	padding: 30px 0;
	border-radius: 10px
}
.icon-item-title {
	margin-top: 12px;
	font-size: 12px;
	font-weight: bold;
	margin-bottom: 6px;
}
.icon-item-caption {
	font-size: 12px;
	color: #cacaca;
}

</style>