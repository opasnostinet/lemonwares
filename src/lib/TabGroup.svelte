<script>
	export let tabNames = [];
	let activeTab = 'Premium';
	
	function onClick(event) {
		activeTab = event.target.textContent.trim();
	}
</script>

<div class="tab-group">
	{#each tabNames as name}
		<span
			class="tab-group_item"
			class:tab-group_item--active={name === activeTab}
			on:click={onClick}>{name}</span
		>
	{/each}
</div>

<style>
	.tab-group {
		border-bottom: 2px grey solid;
		width: 100%;
		display: flex;
	}
	.tab-group_item {
		flex-grow: 1;
		text-align: center;
		position: relative;
		cursor: pointer;
	}
	.tab-group_item--active::after {
		content: '';
		display: block;
		height: 2px;
		width: 100%;
		background-color: #b00000;
		position: absolute;
	}
</style>
