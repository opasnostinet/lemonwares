<script lang="ts">
	import type TariffModel from '../models/tariff';
	import Button from '$lib/Button.svelte';

	export let tariff: TariffModel;
</script>

<article>
	<h3>{tariff.title}</h3>
	<p>{tariff.description}</p>
	<div class="price">{tariff.price}</div>
	<div class="period">{tariff.period}</div>
	<Button secondary={true} width="100%">{tariff.buttonText}</Button>
	<ul>
		{#each tariff.features as feature}
			<li>{feature}</li>
		{/each}
	</ul>
</article>

<style>
	article {
		border-radius: 20px;
		border: #C4C4C4 solid 1px;
		padding: 30px;
		width: 27%;

	}
	ul {
		list-style-image: url(./check.svg);
		margin-top: 35px;
		line-height: 35px;
		padding: 20px;
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
	}

	p {
		font-weight: 400;
		font-size: 12px;
		line-height: 18px;
		margin-bottom: 28px;
	}

	.price {
		font-weight: 600;
		font-size: 42px;
		line-height: 32px;
		margin-bottom: 12px;
	}

	.period {
		font-weight: 300;
		font-size: 14px;
		line-height: 14px;
		margin-bottom: 35px;
	}
</style>
