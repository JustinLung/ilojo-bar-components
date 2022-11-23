<script lang="ts">
	import Button from '$lib/components/Button.svelte';
	export let cardTitle: string = 'Card Title';
	export let cardDescription: string = 'Card Description';
	export let cardImage: string;
</script>

<article>
	<figure>
		<img src={cardImage} alt={cardTitle} />
	</figure>
	<div>
		<h2>{cardTitle}</h2>
		<p>{cardDescription}</p>
		<div>
			<Button>Read More</Button>
		</div>
	</div>
</article>
