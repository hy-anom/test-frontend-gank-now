<template>
	<b-navbar toggleable="lg" type="dark">
		<b-navbar-brand href="#">
			<img class="navbar-logo" src="../assets/logo-gank-red.png">
		</b-navbar-brand>

		<b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

		<b-collapse id="nav-collapse" is-nav>
			<!-- Right aligned nav items -->
			<b-navbar-nav class="ml-auto">
				<b-navbar-nav>
					<b-nav-item href="#">
						<button class="btn btn-navbar">Reserve my profile</button>
					</b-nav-item>
					<b-nav-item href="#" class="navbar-item">Log In</b-nav-item>
					<b-nav-item href="#" class="navbar-item">What's Gank</b-nav-item>
					<b-nav-item href="#" class="navbar-item">Who's on Gank</b-nav-item>
					<b-nav-item-dropdown class="navbar-item" text="EN" right>
						<b-dropdown-item href="#">EN</b-dropdown-item>
						<b-dropdown-item href="#">ES</b-dropdown-item>
						<b-dropdown-item href="#">RU</b-dropdown-item>
						<b-dropdown-item href="#">FA</b-dropdown-item>
					</b-nav-item-dropdown>
				</b-navbar-nav>
			</b-navbar-nav>
		</b-collapse>
	</b-navbar>
</template>

<script>
	export default {

		name: 'Navbar',

		data () {
			return {

			}
		}
	}
</script>

<style lang="scss" scoped>
.navbar-logo {
	height: 30px;
}

.navbar-content {
	display: flex;
}

.btn-navbar {
	background-color: #ED5C5E;
	color: #FFFFFF;
	font-weight: bold;
	font-size: 14px;
	padding: 10px 20px;
	border-radius: 8px;
}

.navbar-dark .navbar-nav .nav-link {
	color: #FFFFFF;
	padding: 10px 24px;
}
.nav-item .navbar-dark .navbar-nav .nav-link {
	color: #FFFFFF;
}
.nav-item.navbar-item {
	display: flex;
	align-items: center;
}

</style>