<div class="portfolio">
	<div>
		<h2>We serve over 100 Nigerian Websites</h2>
		<p>Connect LemonWares with your favourite tools that you use daily and keep things on track.</p>
	</div>
	<div class="clients">
		<img src="logo/jerry-piping.png" alt="JPNL" />
		<img src="logo/korane-scents.png" alt="Korane" />
		<img src="logo/nadine-ghaida.png" alt="NG" />
		<img src="logo/leeve-on-branding.png" alt="LeeveOn" />
		<img src="logo/jrango-glasses.png" alt="JrangGlasses" />
		<img src="logo/crypto-learn-invest.png" alt="CLI" />
	</div>
</div>

<style>
	.portfolio {
		display: grid;
		grid-template-columns: 1fr 1fr;
		gap: 16%;
	}

	.clients {
		display: grid;
		grid-template-columns: repeat(3, minmax(60px, 120px));
		gap: 10px;
		align-items: center;
		justify-content: center;
	}

	h2 {
		font-weight: 800;
		font-size: 48px;
		line-height: 64px;
		color: #18191f;
		margin-bottom: 8px;
	}

	p {
		color: #18191f;
	}

	img {
		width: 100%;
	}

	@media (max-width: 1000px) {
		.portfolio {
			grid-template-columns: 1fr;
			gap: 5%;
		}

		h2 {
			font-size: 38px;
			line-height: 54px;
		}
	}

	@media (max-width: 750px) {
		h2 {
			font-size: 28px;
			text-align: center;
			line-height: 35px;
		}
	}
	@media (max-width: 900px) {
		h2 {
			font-size: 26px;
			line-height: 40px;
		}

		p {
			font-size: 16px;
			line-height: 28px;
		}
	}
</style>
