<script>
	export let secondary = false;
  export let width = "auto";
</script>

<button class:secondary style:width>
	<slot />
</button>

<style>
	button {
		display: flex;
    justify-content: center;
		background-color: #b00000;
		border-radius: 8px;
		padding: 12px 16px;
		align-items: center;
		color: #fff;
		gap: 8px;
		line-height: 24px;
		border: none;
		cursor: inherit;
	}

	.secondary {
		display: flex;
		border-radius: 8px;
    background-color: #fff;
		padding: 12px 16px;
		align-items: center;
		color: #000000;
		gap: 8px;
		line-height: 24px;
		cursor: inherit;
		border: 1px solid #000000;
		box-sizing: border-box;
		border-radius: 8px;

	}
</style>
