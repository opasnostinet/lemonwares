<script lang="ts">
	import type TariffModel from "../models/tariff";
	import Button from "$lib/Button.svelte";

	export let tariff: TariffModel;
	let isExpanded = false;
</script>

<article>
	<h3>{tariff.title}</h3>
	<p>{tariff.description}</p>
	<div class="price">{tariff.price}</div>
	<div class="period">{tariff.period}</div>
	<Button secondary={true} width="100%">{tariff.buttonText}</Button>
	<button class="expand" on:click={() => (isExpanded = !isExpanded)}>
		{isExpanded ? "collapse" : "expand"}
		<svg
			style:transform={isExpanded ? "scale(-1)" : ""}
			class="chevrone"
			viewBox="0 0 10 5"
			fill="none"
		>
			<path
				stroke-linejoin="round"
				stroke-linecap="round"
				stroke="currentColor"
				d="M 1,1 l 4,3 l 4,-3"
			/>
		</svg>
	</button>
	<ul class:hidden={!isExpanded}>
		{#each tariff.features as feature}
			<li>{feature}</li>
		{/each}
	</ul>
</article>

<style>
	article {
		border-radius: 20px;
		border: #c4c4c4 solid 1px;
		padding: 30px;
		width: 27%;
		box-sizing: border-box;
		gap: 12px;
		display: grid;
	}
	ul {
		display: grid;
		grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
		list-style-image: url(/check.svg);
		margin-top: 15px;
		margin-bottom: initial;
		line-height: 35px;
		list-style-position: inside;
	}
	li {
		color: #808080;
		padding-left: 20px;
	}

	h3 {
		margin-top: 0;
		font-weight: 600;
		font-size: 28px;
		line-height: 25px;
		margin-bottom: 8px;
	}
	.hidden {
		display: none;
	}

	.chevrone {
		width: 20px;
		height: auto;
		transition: transform 0.3s;
	}

	p {
		font-weight: 400;
		font-size: 12px;
		line-height: 18px;
		margin: 0;
	}

	.price {
		font-weight: 600;
		font-size: 42px;
		line-height: 32px;
	}

	.period {
		font-weight: 300;
		font-size: 14px;
		line-height: 14px;
		margin-bottom: 12px;
	}

	button {
		display: flex;
		color: #b00000;
		border-radius: 8px;
		padding: 12px 16px;
		align-items: baseline;
		background-color: #fff;
		line-height: 24px;
		border: none;
		cursor: inherit;
		width: 100%;
		display: inline-block;
	}

	@media (max-width: 1200px) {
		article {
			width: initial;
		}

		ul {
			padding: 0;
		}
	}
	@media (max-width: 900px) {
		h3 {
			font-size: 24px;
			line-height: 24px;
		}
		p,
		.period {
			font-size: 16px;
			line-height: 28px;
		}
		.price {
			font-size: 30px;
			line-height: 32px;
		}
	}

	@media (min-width: 900px) {
		.expand {
			display: none;
		}
		.hidden {
			display: block;
		}

		ul {
			margin: initial;
		}
	}
</style>
