<template>
	<swiper class="swiper" :options="swiperOption">
		<swiper-slide>
			<slider-item
				img-src="player-niko.png"
				name="Nikobaby"
				desc="Alliance's carry player on Dota 2. Also known as prison RTZ"
				:pro="true"
			></slider-item>
		</swiper-slide>
		<swiper-slide>
			<slider-item
				img-src="player-limpp.png"
				name="Limpp"
				desc="Alliance's mid player on Dota 2"
				:pro="true"
			></slider-item>
		</swiper-slide>
		<swiper-slide>
			<slider-item
				img-src="player-s4.png"
				name="s4"
				desc="Alliance's offlane player on Dota 2"
			></slider-item>
		</swiper-slide>
		<swiper-slide>
			<slider-item
				img-src="player-handsken.png"
				name="Handsken"
				desc="Alliance's support player on Dota 2"
				:pro="true"
			></slider-item>
		</swiper-slide>
		<swiper-slide>
			<slider-item
				img-src="player-fng.png"
				name="FNG"
				desc="Alliance's support player on Dota 2"
			></slider-item>
		</swiper-slide>

		<div class="swiper-pagination" slot="pagination"></div>
	</swiper>
</template>

<script>
import SliderItem from './SliderItem';
import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper';
import 'swiper/swiper-bundle.css';

export default {
	name: 'Slider',
	components: {
		SliderItem,
		Swiper,
		SwiperSlide
	},
	directives: {
		swiper: directive
	},

	data () {
		return {
		}
	},

	computed: {
		swiperOption() {
			return {
				slidesPerView: 
					window.innerWidth > 480 ? window.innerWidth > 720 ? 4 : 2 : 1,
				spaceBetween: 20,
				pagination: {
					el: '.swiper-pagination',
					clickable: true
				}
			}
		}
	}
}
</script>

<style lang="scss" scoped>
</style>