<script>
	import Button from './Button.svelte';
</script>

<section>
	<div>
		<ul>
			<li>Hosting</li>
			<li>Domain</li>
			<li>SEO</li>
			<li>Email</li>
		</ul>

		<h1>Premium Web Hosting for Your Website</h1>
		<p>
			Blazing fast web hosting for individuals and businesses of all sizes backed by 24x7x365
			Support.
		</p>
		<div class="buttons">
			<Button>Create an Account</Button>
			<Button secondary={true}>Choose your plan</Button>
		</div>
	</div>

	<div class="img-wrapper">
		<div class="img-sub-wrapper">
			<img class="hero" src="/logo/person-with-notebook.png" alt="person-with-notebook" />
			<img class="triangle triangle-1" src="icon/triangle.svg" alt="" />
			<img class="triangle triangle-2" src="icon/triangle.svg" alt="" />
			<img class="triangle triangle-3" src="icon/triangle.svg" alt="" />
		</div>
	</div>
</section>

<style>
	ul {
		display: flex;
		list-style-type: none;
		margin: 0;
		padding: 0;
		font-weight: 600;
		font-size: 15px;
		line-height: 22px;
		gap: 15px;
		color: #d6d4d4e0;
		position: relative;
	}

	ul:after {
		display: block;
		content: '';
		background: #d6d4d4e0;
		height: 2px;
		position: absolute;
		width: 67%;
		bottom: -4px;
		left: 5px;
	}
	ul li:first-child {
		color: #b00000;
	}

	li:hover:after {
		content: '';
		width: 80%;
		height: 2px;
		background: #b00000;
		display: block;
		position: absolute;
		bottom: -4px;
		left: 10%;
		z-index: 1;
	}
	li {
		flex-shrink: 0;
		position: relative;
	}
	.hero {
		display: block;
		width: 100%;
	}

	.img-wrapper {
		width: 80%;
	}

	.img-sub-wrapper {
		position: relative;
	}

	section {
		display: flex;
		margin: 50px 110px;
		gap: 50px;
	}

	h1 {
		font-weight: 700;
		font-size: 64px;
		line-height: 78px;
		margin: 26px 0 34px;
	}

	p {
		font-weight: 400;
		font-size: 16px;
		line-height: 28px;
		color: #808080;
		margin-bottom: 60px;
		width: 73%;
	}

	.buttons {
		display: flex;
		gap: 24px;
	}

	.triangle {
		position: absolute;
	}

	.triangle-1 {
		right: -7%;
		bottom: 8%;
		width: 14%;
		height: 14%;
	}

	.triangle-2 {
		left: -5%;
		bottom: 33%;
		transform: scaleX(-1);
		width: 8%;
		height: 8%;
	}

	.triangle-3 {
		top: 11%;
		left: 97%;
		width: 8%;
		height: 8%;
	}

	@media (max-width: 1050px) {
		.img-wrapper {
			display: none;
		}

		h1 {
			font-weight: 700;
			font-size: 39px;
			line-height: initial;
		}

		section {
			margin: 25px 55px;
		}
	}
	@media (max-width: 900px) {
		h1 {
			margin: 14px 0 20px;
			font-size: 30px;
			line-height: 40px;
		}
	}

	@media (max-width: 650px) {
		section {
			margin: 25px 25px;
		}

		.buttons {
			flex-direction: column;
		}

		p {
			margin-bottom: 20px;
			width: 100%;
		}
	}
</style>
