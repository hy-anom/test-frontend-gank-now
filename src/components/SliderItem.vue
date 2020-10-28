<template>
	<div>
		<div class="slider-item">
			<div class="profile-picture">
				<img :src="require(`@/assets/players/${imgSrc}`)">
			</div>
			<p class="profile-name">
				{{ name }}
				<span v-if="pro" class="profile-pro">
					<img src="../assets/ic-crown.png">
					<span>PRO</span>
				</span>
			</p>
			<p class="profile-desc">
				{{ desc }}
			</p>	
		</div>

	</div>
</template>

<script>
export default {
  name: 'SliderItems',

  props: {
    imgSrc: {
      type: String,
    },
    name: {
      type: String,
    },
    pro: {
    	type: Boolean,
    },
    desc: {
      type: String,
    },
  }
}
</script>

<style lang="scss" scoped>
.slider-item {
	display: flex;
	flex-direction: column;
	align-items: center;
	background-color: #393E5E;
	padding: 20px 10px;
	border-radius: 8px;
	height: 240px;
}

.profile-picture {
	height: 100px;
	width: 100px;

	img {
		height: 100%;
		width: 100%;
		border-radius: 100%;
	}
}

.profile-name {
	margin-top: 10px;
	margin-bottom: 8px;
}

.profile-desc {
	font-size: 12px;
	text-align: center;
}

.profile-pro {
	display: inline-flex;
	background-color: #000000;
	font-size: 8px;
	border-radius: 100px;
	padding: 2px 6px;
	align-items: center;

	img {
		margin-right: 4px;
		margin-top: -3px;
	}
}
</style>