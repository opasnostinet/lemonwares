<script lang="ts">
	import type TariffModel from '../models/tariff';

	export let tariff: TariffModel;
</script>

<article>
	<h3>{tariff.title}</h3>
	<p>{tariff.description}</p>
	<div>{tariff.price}</div>
	<div>{tariff.period}</div>
	<input type="button" value={tariff.buttonText} />
	<ul>
		{#each tariff.features as feature}
			<li>{feature}</li>
		{/each}
	</ul>
</article>

<style>
	article {
		border-radius: 20px;
		border: black solid 1px;
    padding: 20px;
	}
	ul {
		list-style-image: url(./check.svg);
	}

  h3{
    margin-top: 0;
  }
</style>
