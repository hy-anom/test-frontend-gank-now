<template>
	<section class="features">
		<div class="feature-row">
			<div class="feature-content-wide">
				<div class="image-container">
					<img src="../assets/img-screen.png">
				</div>
			</div>
			<div class="feature-content">
				<div class="feature-text">
					<p class="feature-title">Showcase your best moments</p>
					<p class="feature-caption">
						Curate and share your best gaming moment on your profile.
					</p>
				</div>
			</div>
		</div>

		<div class="feature-row">
			<div class="feature-content">
				<div class="feature-text">
					<p class="feature-title">
						Unveil your strengths in  the game
					</p>
					<p class="feature-caption">
						Are you a carry, support or jungler? Or are you a DPS, healer or tank? Share these specialisations on your profile.
					</p>
				</div>
			</div>
			<div class="feature-content-wide">
				<div class="feature-chart-container">
					<features-chart></features-chart>
				</div>
			</div>
		</div>


		<div class="feature-row">
			<div class="feature-content-wide">
				<div class="feature-achievement">
					<p class="achievement-title">ACHIEVEMENT</p>
					<div class="achievement-list">
						<div class="achievement-icon">
							<img src="../assets/ic-dota2.png">
						</div>
						<div class="achievement-text">
							<p class="achievement-text-title">1st Place</p>
							<p class="achievement-text-subtitle">
								Dota 2 Asia Championship
							</p>
						</div>
					</div>
					<div class="achievement-list">
						<div class="achievement-icon">
							<img src="../assets/ic-dota2.png">
						</div>
						<div class="achievement-text">
							<p class="achievement-text-title">4th - 5th Place</p>
							<p class="achievement-text-subtitle">
								The International 5
							</p>
						</div>
					</div>
					<div class="achievement-list">
						<div class="achievement-icon">
							<img src="../assets/ic-dota2.png">
						</div>
						<div class="achievement-text">
							<p class="achievement-text-title">1st Place</p>
							<p class="achievement-text-subtitle">
								Dota 2 Asia Championship
							</p>
						</div>
					</div>
				</div>
			</div>
			<div class="feature-content">
				<div class="feature-text">
					<p class="feature-title">A place for all your achievements</p>
					<p class="feature-caption">
						List out the competitive achievements you have won and let the world know.
					</p>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
import FeaturesChart from './FeaturesChart.vue';

export default {
  name: 'Features',
	components: {
    FeaturesChart,
  },
  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.features {
	padding: 0 20px;
	max-width: 800px;
	margin: auto;
}

.feature-row {
	display: flex;
	margin-top: 40px;
	flex-wrap: wrap;
}
.feature-content-wide {
	flex: 3;

	@media (max-width: 640px) {
		flex-basis: 100%;
	}
}
.feature-content {
	flex: 2;
	@media (max-width: 640px) {
		flex-basis: 100%;
		order: 2;
	}
}

.image-container {
	width: 400px;
	@media (max-width: 640px) {
		width: 100%;
	}

	img {
		height: 100%;
		width: 100%;
	}
}


.feature-text {
	width: 240px;
	margin: 90px auto;

	@media (max-width: 640px) {
		margin: 30px auto;
	}
}
.feature-title {
	font-size: 24px;
	margin-bottom: 14px;
	line-height: 1.2;
}
.feature-caption {
	font-size: 12px;
}


.feature-achievement {
	background-color: #393E5E;
	border-radius: 10px;
	padding: 20px 30px 10px;
	width: 400px;
	@media (max-width: 640px) {
		width: 100%;
	}
}

.achievement-title {
	color: #717696;
	font-size: 18px;
	font-weight: bold;
}
.achievement-list {
	display: flex;
	margin-bottom: 16px;
}
.achievement-icon {
	width: 40px;
	margin-right: 36px;
	height: 46px;
	img {
		height: 100%;
	}
}
.achievement-text {
	p {
		margin: 0;
	}

	.achievement-text-subtitle {
		color: #717696;
	}
}
</style>