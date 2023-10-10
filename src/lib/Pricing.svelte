<script lang="ts">
	import Toggler from '$lib/Toggler.svelte';
	import TabGroup from '$lib/TabGroup.svelte';
	import Tariff from '$lib/Tariff.svelte';
	import type TariffModel from '../models/tariff';

	let tariffList: TariffModel[] = [
		{
			title: 'Starter',
			description:
				'with all your customers via all conversation channels in one central dashboard.',
			price: '$2.80',
			period: 'Per month',
			buttonText: 'Choose this Plan',
			features: [
				'2GB SSD',
				'10GB Bandwidth',
				'15 Email Accounts',
				'Unlimited Database',
				'4 Subdomains',
				'1 Parked Domain',
				'2 Websites',
				'Free SSL',
				'Softaculous'
			]
		},
		{
			title: 'Standard',
			description:
				'with all your customers via all conversation channels in one central dashboard.',
			price: '$4.20',
			period: 'Per month',
			buttonText: 'Choose this Plan',
			features: [
				'2GB SSD',
				'10GB Bandwidth',
				'15 Email Accounts',
				'Unlimited Database',
				'4 Subdomains',
				'1 Parked Domain',
				'2 Websites',
				'Free SSL',
				'Softaculous'
			]
		},
		{
			title: 'Suprem',
			description:
				'with all your customers via all conversation channels in one central dashboard.',
			price: '$7.00',
			period: 'Per month',
			buttonText: 'Choose this Plan',
			features: [
				'2GB SSD',
				'10GB Bandwidth',
				'15 Email Accounts',
				'Unlimited Database',
				'4 Subdomains',
				'1 Parked Domain',
				'2 Websites',
				'Free SSL',
				'Softaculous'
			]
		}
	];
</script>

<section class="wrapper">
	<h2>Ready to get started with Lemon Wares?</h2>
	<p>Choose the package that suits you</p>
	<div class="toggler_wrapper">
		<Toggler option1="Monthly" option2="Yearly" small="30% discount" />
	</div>
	<div class="tab-group-wrapper">
		<TabGroup tabNames={['Basic', 'Premium']} />
	</div>
	<div class="tariff-wrapper">
		{#each tariffList as tariff}
			<Tariff {tariff} />
		{/each}
	</div>
</section>

<style>
	h2 {
		font-weight: 600;
		font-size: 50px;
		line-height: 60px;
		max-width: 650px;
		text-align: center;
		margin-bottom: 0;
	}
	p {
		font-weight: 400;
		font-size: 25px;
		line-height: 25px;
		margin-bottom: 25px;
	}
	.wrapper {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		margin: 5%;
		gap: 35px;
	}
	.toggler_wrapper {
		margin-bottom: 50px;
	}

	.tab-group-wrapper {
		width: 80%;
		margin-bottom: 5px;
	}

	.tariff-wrapper {
		display: flex;
		gap: 100px;
	}

	@media (max-width: 1200px) {
		.tariff-wrapper {
			gap: 5%;
			align-items: center;
		}
		.tab-group-wrapper {
			display: none;
		}
		.toggler_wrapper {
			margin-bottom: 20px;
		}
	}
	@media (max-width: 900px) {
		.tariff-wrapper {
			flex-direction: column;
			gap: 50px;
		}

		.wrapper {
			gap: 10px;
		}
		h2 {
			margin: 0;
			font-size: 40px;
		}
	}
</style>
