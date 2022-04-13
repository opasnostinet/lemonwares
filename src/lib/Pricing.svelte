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
	<Toggler option1="Monthly" option2="Yearly" small="30% discount" />
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
	.wrapper {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
		margin: 5%;
	}

	.tab-group-wrapper {
		width: 80%;
		margin-bottom: 40px;
	}

	.tariff-wrapper {
		display: flex;
		gap: 40px;
	}
</style>
