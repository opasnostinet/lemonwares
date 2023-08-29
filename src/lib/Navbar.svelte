<script>
	let isMenuVisible = false;
	function openMenu() {
		isMenuVisible = true;
	}
	function closeMenu() {
		isMenuVisible = false;
	}
</script>

<nav>
	<img class="logo" src="logo/logo.png" alt="logo" />

	<ul class="desktop-links">
		<li><a href="/">Our Services</a></li>
		<li><a href="/">About</a></li>
		<li><a href="/">Blog&News</a></li>
		<li><a href="/">Contact</a></li>
		<li><a href="/">Account</a></li>
	</ul>

	<img class="phone-icon" src="icon/phone.svg" alt="phone" />
	<a class="phone-link" href="tel:+2349067322844">+2349067322844</a>

	<h1 class="mobile-title">Lemonwares</h1>
	<button class="menu-button" on:click={openMenu}>
		<img class="menu-icon" src="icon/menu.svg" alt="menu" />
	</button>
	<div class="overlay overlay--active" class:overlay--active={isMenuVisible}>
		<div class="menu">
			<ul class="mobile-links">
				<li><a href="/">Our Services</a></li>
				<li><a href="/">About</a></li>
				<li><a href="/">Blog&News</a></li>
				<li><a href="/">Contact</a></li>
				<li><a href="/">Account</a></li>
			</ul>
			<button class="close" on:click={closeMenu}>
				<img src="icon/close.svg" alt="close" />
			</button>
		</div>
	</div>
</nav>

<style>
	nav {
		display: flex;
		margin: 40px 190px 40px 110px;
		align-items: center;
		font-weight: 600;
		font-size: 15px;
		line-height: 22px;
	}

	.desktop-links {
		display: flex;
		flex-grow: 1;
		list-style-type: none;
		padding: 0;
		gap: 4.4%;
	}

	.desktop-links li:first-child {
		margin-right: auto;
	}

	.desktop-links li:last-child {
		margin-left: auto;
	}

	.desktop-links:after {
		height: 21px;
		width: 2px;
		background-color: #dad8d8;
		display: block;
		content: '';
		margin-right: 43px;
	}

	.desktop-links li:hover:after {
		content: '';
		width: 80%;
		height: 2px;
		background: #b00000;
		display: block;
		position: absolute;
		bottom: -5px;
		left: 10%;
	}

	.desktop-links li {
		flex-shrink: 0;
		position: relative;
	}

	.logo {
		margin-right: 65px;
	}

	a {
		text-decoration: none;
		color: #000000;
	}
	.phone-icon {
		margin-right: 6px;
		width: 20px;
	}

	.menu-button,
	.mobile-title,
	.overlay {
		display: none;
	}

	.overlay {
		background-color: hsla(0, 0%, 7%, 0.36);
		backdrop-filter: blur(4px);
		position: fixed;
		z-index: 1;
		top: 0;
		left: 0;
		width: 100vw;
		height: 100vh;
	}
	.overlay--active {
		display: block;
	}

	.mobile-links {
		padding: 0;
		margin: 0;
		list-style-type: none;
		display: flex;
		flex-direction: column;
		gap: 15px;
	}

	.mobile-links li {
		padding: 10px 0;
	}
	.menu {
		background: #fff;
		width: 320px;
		height: 100%;
		margin-left: auto;
		padding: 50px;
		box-sizing: border-box;
	}

	.close {
		position: absolute;
		top: 0;
		right: 0;
		padding: 15px;
		background: none;
		border: none;
	}

	@media (max-width: 1050px) {
		.desktop-links,
		.phone-icon,
		.phone-link {
			display: none;
		}

		.mobile-title,
		.menu-button {
			display: block;
		}
		.mobile-title {
			font-size: 30px;
			font-weight: 400;
		}

		nav {
			margin: 15px 30px;
			justify-content: space-between;
		}

		.logo {
			margin: 0;
			width: 65px;
		}

		.menu-button {
			background: none;
			border: none;
		}

		.menu-icon {
			display: block;
		}
	}

	@media (max-width: 400px) {
		.mobile-title {
			font-size: 20px;
		}

		nav {
			margin: 10px;
		}
	}
</style>
