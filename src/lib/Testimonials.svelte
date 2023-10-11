<div class="quotes">
	<article class="quote">
		<img class="quote-mark" src="quote-mark.svg" alt="quotes" />
		<h2>Real Stories from Real Customers</h2>
		<span>Get inspired by these stories.</span>
	</article>
	<article class="quote">
		<img src="logo/crypto-learn-invest.png" alt="CLI" />
		<blockquote>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta excepturi repellendus dolores
				magni quaerat molestias? Hic fuga consectetur itaque qui ab asperiores repellat, pariatur
				labore praesentium? Dolorem ipsam rerum enim.
			</p>
			<cite>Floyd Miles</cite>
			<div class="author">Vice President, CLI</div>
		</blockquote>
	</article>
	<article class="quote">
		<img src="logo/jerry-piping.png" alt="JPNL" />
		<blockquote>
			<p>
				Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta excepturi repellendus dolores
				magni quaerat molestias? Hic fuga consectetur itaque qui ab asperiores repellat, pariatur
				labore praesentium? Dolorem ipsam rerum enim.
			</p>
			<cite>Jane Cooper</cite>
			<div class="author">SEO, JPNL</div>
		</blockquote>
	</article>
	<article class="quote">
		<img src="logo/leeve-on-branding.png" alt="LeeveOn" />
		<blockquote>
			<p>LemonWares saved our time in Hosting my company page.</p>
			<cite>Kristin Watson</cite>
			<div class="author">Co-Founder, LeeveOn Branding</div>
		</blockquote>
	</article>
</div>

<style>
	img {
		display: block;
	}

	p {
		margin: 0 0 24px;
	}

	h2 {
		font-weight: 800;
		font-size: 48px;
		line-height: 64px;
		color: #18191f;
		margin-bottom: 8px;
	}

	span {
		font-weight: 400;
		font-size: 18px;
		line-height: 32px;
		color: #18191f;
	}

	cite {
		font-weight: 700;
		font-size: 18px;
		line-height: 28px;
		font-style: normal;
		color: #18191f;
	}

	.author {
		font-weight: 500;
		font-size: 14px;
		line-height: 24px;
		color: #969bab;
	}
	blockquote {
		margin: 0;
	}
	.quotes {
		display: flex;
		flex-direction: column;
		flex-wrap: wrap;
		gap: 0 30px;
		align-content: center;
		max-height: 818px;
	}
	.quote {
		line-height: 32px;
		max-width: 445px;
		padding: 32px 32px 32px 64px;
		box-sizing: border-box;
		box-shadow: 0px 10px 20px rgba(41, 41, 42, 0.07);
		border-radius: 8px;
	}

	.quote:first-child {
		padding: initial;
		position: relative;
		box-shadow: none;
	}

	.quote:first-child h2 {
		font-size: 42px;
		line-height: 60px;
	}

	.quote:nth-child(2) {
		place-self: end;
	}

	.quote:nth-child(2),
	.quote:nth-child(4) {
		max-width: 350px;
	}

	.quote:nth-child(3) {
		margin-top: 50px;
		margin-bottom: 34px;
	}

	.quote-mark {
		position: absolute;
		top: -25px;
		left: -95px;
	}

	@media (max-width: 1100px) {
		.quotes {
			max-height: initial;
		}
		.quote {
			max-width: initial;
			padding: 32px;
		}
		.quote:nth-child(2),
		.quote:nth-child(4) {
			max-width: initial;
		}
		.quote:first-child h2 {
			font-size: 35px;
		}
	}

	@media (max-width: 970px) {
		.quotes {
			max-height: initial;
		}
		.quote {
			padding: 1em;
		}
	}

	@media (max-width: 900px) {
		.quote-mark {
			display: none;
		}

		.quote:first-child h2 {
			line-height: 45px;
		}

		.quote {
			line-height: 25px;
		}
	}
</style>
