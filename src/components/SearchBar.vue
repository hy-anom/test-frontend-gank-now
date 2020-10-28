<template>
	<div class="search-bar">
		<input type="text" name="search-bar" placeholder="ganknow.com/pewpewpew">
		<button class="btn">
			<img src="../assets/btn-arrow-red.png">
		</button>
	</div>
</template>

<script>
export default {

  name: 'SearchBar',

  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
	.search-bar {
		background-color: #ffffff;
		width: 400px;
		border-radius: 8px;
		display: flex;
		align-items: center;
		justify-content: space-between;
		padding: 3px 4px;

		input	{
			border: none;
			height: 40px;
			width: 100%;
			margin: 0 10px;
			font-size: 14px;
		}
		.btn {
			padding: 0;
			img	{
				height: 40px;

			}
		}
	}
	
</style>