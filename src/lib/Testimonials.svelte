<div class="quotes">
	<article class="quote">
		<img class="quote-mark" src="quote-mark.svg" alt="quotes" />
		<h2>Real Stories from Real Customers</h2>
		<div>Get inspired by these stories.</div>
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
			<div>Vice President, CLI</div>
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
			<div>SEO, JPNL</div>
		</blockquote>
	</article>
	<article class="quote">
		<img src="logo/leeve-on-branding.png" alt="LeeveOn" />
		<blockquote>
			<p>LemonWares saved our time in Hosting my company page.</p>
			<cite>Kristin Watson</cite>
			<div>Co-Founder, LeeveOn Branding</div>
		</blockquote>
	</article>
</div>


<style>
	img {
		display: block;
	}

	p {
		margin: 0;
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
		max-height: 720px;
	}

	@media (max-width: 970px) {
		.quotes {
			max-height: initial;
		}
	}

	.quote {
		line-height: 32px;
		max-width: 445px;
		padding: 32px 32px 32px 64px;
		box-sizing: border-box;
	}

	.quote:first-child {
		padding: initial;
		position: relative;
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
	}

	.quote-mark {
		position: absolute;
		top: -25px;
		left: -95px;
	}


</style>
