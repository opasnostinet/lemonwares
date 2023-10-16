<script>
	export let option1;
	export let option2;
	export let small;
</script>

<label class="switch">
	<input type="checkbox" />
	{option1}
	<div class="slider round" />
	{option2}
	<small>{small}</small>
</label>

<style>
	.switch {
		display: flex;
		align-items: center;
		gap: 15px;
	}

	.switch input {
		opacity: 0;
		width: 0;
		height: 0;
		position: absolute;
	}

	.slider {
		width: 93px;
		height: 50px;
		cursor: pointer;
		background-color: #b0000052;
		-webkit-transition: 0.4s;
		transition: 0.4s;
		position: relative;
	}

	.slider:before {
		position: absolute;
		content: '';
		height: 30px;
		width: 30px;
		left: 11px;
		bottom: 10px;
		background-color: white;
		-webkit-transition: 0.4s;
		transition: 0.4s background-color, 0.4s transform;
	}

	input:checked + .slider {
		background-color: #b00000;
	}

	input:checked + .slider:before {
		transform: translateX(41px);
	}

	/* Rounded sliders */
	.slider.round {
		border-radius: 34px;
	}

	.slider.round:before {
		border-radius: 73px;
	}

	small {
		padding: 5px;
		background-color: #ffe87a;
		border-radius: 8px;
		font-size: 10px;
	}

	@media (max-width: 900px) {
		.slider {
			width: 69px;
			height: 35px;
			border-radius: 34px;
			flex-shrink: 0;
		}
		.slider:before {
			height: 20px;
			width: 20px;
			bottom: 8px;
		}
		input:checked + .slider:before {
			transform: translateX(27px);
		}
		.switch {
			gap: 10px;
		}
	}
</style>
