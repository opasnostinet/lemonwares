<script>
	import Button from './Button.svelte';
</script>

<section>
	<h2>We're here to make your website awesome.</h2>
	<a href="/">
		<Button>
			<img class="whatsapp-icon" src="icon/whats-up.svg" alt="whatsapp" />
			<span>Get in touch with us</span>
		</Button>
	</a>
	<img class="triangle triangle-1" src="icon/triangle.svg" alt="" />
	<img class="triangle triangle-2" src="icon/triangle.svg" alt="" />
	<img class="triangle triangle-3" src="icon/triangle.svg" alt="" />
</section>

<style>
	section {
		display: flex;
		justify-content: center;
		flex-direction: column;
		align-items: center;
		background-color: #f7fafe;
		padding: 80px 90px;
		position: relative;
	}

	h2 {
		width: 80%;
		margin-top: 0;
		margin-bottom: 40px;
		text-align: center;
		font-weight: 600;
		font-size: 64px;
		line-height: 88px;
		color: #2e2e2e;
	}

	.whatsapp-icon {
		width: 25px;
		height: 25px;
	}

	.triangle {
		position: absolute;
	}

	.triangle-1 {
		right: -15px;
		bottom: 30px;
	}

	.triangle-2 {
		left: -10px;
		bottom: 70px;
		transform: scaleX(-1);
		width: 40px;
		height: 40px;
	}

	.triangle-3 {
		top: 0px;
		left: 200px;
		width: 40px;
		height: 40px;
	}
	a {
		text-decoration: none;
		cursor: pointer;
	}
</style>
