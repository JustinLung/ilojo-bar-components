<script type="ts">
	import { onMount } from 'svelte';

	let time = new Date();

	$: hours = time.getHours();
	$: minutes = time.getMinutes();
	$: seconds = time.getSeconds();

	onMount(() => {
		const interval = setInterval(() => {
			time = new Date();
		}, 1000);
    
		return () => {
			clearInterval(interval);
		};
	});
</script>

<svg viewBox='-50 -50 100 100'>
	<circle class='clock-circle' r='48'/>
	{#each [0, 5, 10, 15, 20, 25, 30, 35, 40, 45, 50, 55] as minute}
		<line
			class='hour-lines'
			y1='35'
			y2='45'
			transform='rotate({30 * minute})'
		/>

		{#each [1, 2, 3, 4] as offset}
			<line
				class='minute-lines'
				y1='42'
				y2='45'
				transform='rotate({6 * (minute + offset)})'
			/>
		{/each}
	{/each}

	<line
		class='hour'
		y1='2'
		y2='-20'
		transform='rotate({30 * hours + minutes / 2})'
	/>

	<line
		class='minute'
		y1='4'
		y2='-30'
		transform='rotate({6 * minutes + seconds / 10})'
	/>

	<g transform='rotate({6 * seconds})'>
		<line class='second' y1='10' y2='-38'/>
	</g>
</svg>

<style>
	svg {
		width: 10em;
		height: 10em;
	}

	.clock-circle {
		stroke: #000;
		fill: #fff;
	}

	.minute-lines {
		stroke: #000;
		stroke-width: 1;
	}

	.hour-lines {
		stroke: #000;
		stroke-width: 1.5;
	}

	.hour {
		stroke: #000;
		stroke-width: 1.5;
	}

	.minute {
		stroke: #000;
		stroke-width: 1.5;
	}

	.second {
		stroke: red;
		stroke-width: 1.5;
	}
</style>