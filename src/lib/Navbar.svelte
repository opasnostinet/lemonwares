<nav>
	<img class="logo" src="logo/logo.png" alt="logo" />

	<ul>
		<li>Our Services</li>
		<li>About</li>
		<li>Blog&News</li>
		<li>Contact</li>
		<li>Account</li>
	</ul>

	<img class="phone" src="icon/phone.svg" alt="phone" style="width:20px" />
	<a href="tel:+2349067322844">+2349067322844</a>
</nav>

<style>
	nav {
		display: flex;
		margin: 40px 110px;
		align-items: center;
		font-weight: 600;
		font-size: 15px;
		line-height: 22px;
	}

	ul {
		display: flex;
		flex-grow: 1;
		list-style-type: none;
		padding: 0;
		gap: 4.4%;
	}

	ul li:first-child {
		margin-right: auto;
	}

	ul li:last-child {
		margin-left: auto;
	}

	ul:after {
		height: 21px;
		width: 2px;
		background-color: #dad8d8;
		display: block;
		content: '';
		margin-right: 43px;
	}

	li:hover:after {
		content: '';
		width: 80%;
		height: 2px;
		background: #b00000;
		display: block;
		position: absolute;
		bottom: -5px;
		left: 10%;
	}

	li {
		flex-shrink: 0;
		position: relative;
	}

	.logo {
		display: block;
		margin-right: 65px;
	}

	a {
		text-decoration: none;
		color: #000000;
	}
	.phone {
		margin-right: 6px;
	}
</style>
