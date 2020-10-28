<template>
	<section class="footer">
    <div class="logo-container">
      <img src="../assets/logo-gank-blue.png">
    </div>
    <div class="footer-text">
      <p>2020 &copy; Allright reserved. Gank Global Pte. Ltd</p>
      <p>hello@gankglobal.com</p>
    </div>
	</section>
</template>

<script>
export default {
  name: 'Footer',

  data () {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
.footer {
	display: flex;
	justify-content: space-between;
	padding: 20px 0;
	margin: 60px 20px 0;
	border-top: 1px solid #393E5E;
}

.logo-container {
	height: 24px;

	img	{
		height: 100%;
	}
}

.footer-text {
	p {
		font-size: 10px;
		color: #999;
		margin-bottom: 2px;
		text-align: right;
	}
}
</style>