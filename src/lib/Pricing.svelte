<script>
	import Toggler from '$lib/Toggler.svelte';
</script>

<section class="wrapper">
	<h2>Ready to get started with Lemon Wares?</h2>
	<Toggler option1="Monthly" option2="Yearly" small="30% discount" />
	<ul>
		<li>Basic</li>
		<li>Premium</li>
	</ul>
	<ul>
		<li>Starter</li>
		<li>Standart</li>
		<li>Suprem</li>
	</ul>
</section>

<style>
	.wrapper {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}
</style>
