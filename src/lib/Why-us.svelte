<section>
	<div class="description">
		<h2>True Cloud Web Hosting</h2>
		<p>
			True Cloud Web Hosting All of the hosting packages we offer are deployed instantly on our SSD
			powered cloud. We don't use dedicated servers that operate on single pieces of hardware. Our
			entire infrastructure is built to be reliable, secure, and scalable.
		</p>
	</div>
	<div class="partners">
		<img src="logo/cpanel.png" alt="cPanel" />
		<img src="logo/imunify360.png" alt="imunifi" />
		<img src="logo/litespeed.png" alt="LiteSpeed" />
		<img src="logo/softaculous.png" alt="Softaculous" />
		<img src="logo/word-press.png" alt="WordPress" />
		<img src="logo/cloudflare.png" alt="CloudFlare" />
	</div>
</section>

<ul class="advantages">
	<li class="advantages_item">
		<img class="advantages_img" src="icon/clock.svg" alt="uptime" />
		<h4 class="advantages_title">99,9% Uptime</h4>
		<p class="advantages_description">
			We Keep Your Web build Online 24x7x365. Downtime not only costs you lost visitors but also
			damages your reputation and search engine rankings.
		</p>
	</li>
	<li class="advantages_item">
		<img class="advantages_img" src="icon/setting.svg" alt="web-hosting" />
		<h4 class="advantages_title">Blazing Fast Web Hosting</h4>
		<p class="advantages_description">
			We Keep Your Web build Online 24x7x365. Downtime not only costs you lost visitors but also
			damages your reputation and search engine rankings.
		</p>
	</li>
	<li class="advantages_item">
		<img class="advantages_img" src="icon/certificate.svg" alt="certificates" />
		<h4 class="advantages_title">Free SSL Certificates</h4>
		<p class="advantages_description">
			We Keep Your Web build Online 24x7x365. Downtime not only costs you lost visitors but also
			damages your reputation and search engine rankings.
		</p>
	</li>
	<li class="advantages_item">
		<img class="advantages_img" src="icon/support.svg" alt="support" />
		<h4 class="advantages_title">24x7 Friendly Support</h4>
		<p class="advantages_description">
			We Keep Your Web build Online 24x7x365. Downtime not only costs you lost visitors but also
			damages your reputation and search engine rankings.
		</p>
	</li>
</ul>

<style>
	section {
		display: flex;
		margin: 80px 76px;
		gap: 70px;
	}

	h2 {
		font-weight: 800;
		font-size: 48px;
		line-height: 64px;
		font-family: Inter;
	}

	h4 {
		font-weight: 700;
		font-size: 20px;
		line-height: 30px;
		margin: 20px auto 6px;
	}

	.description {
		width: 46%;
	}

	.description p {
		color: #18191f;
		font-weight: 400;
		font-size: 18px;
		line-height: 32px;
	}
	.advantages {
		display: flex;
		list-style-type: none;
		margin: 0;
		text-align: center;
		gap: 60px;
		justify-content: center;
		padding: 0;
	}

	.advantages_item {
		max-width: 270px;
	}
	.advantages_img {
		width: 100px;
	}

	img {
		width: 100%;
	}

	.partners {
		display: grid;
		grid-template-columns: 1fr 1fr 1fr;
		grid-template-rows: 70px;
		grid-auto-rows: 50px;
		gap: 60px 65px;
		flex-shrink: 0;
		align-items: center;
		align-content: center;
		justify-items: center;
	}

	.advantages_description {
		font-weight: 300;
		font-size: 12px;
		line-height: 18px;
		text-align: center;
	}

	@media (max-width: 1200px) {
		section {
			flex-direction: column;
			margin: 40px 24px;
			gap: 10px;
		}
		.description {
			width: auto;
		}

		h2 {
			font-size: 29px;
			font-weight: 700;
			line-height: initial;
		}

		.advantages {
			flex-direction: column;
			align-items: center;
			gap: 30px;
		}

		img {
			max-width: 150px;
		}

		.partners {
			gap: 10px 15px;
		}
	}
</style>
