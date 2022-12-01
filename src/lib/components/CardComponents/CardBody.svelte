<script lang="ts">
	export let cardTitle: string = 'Title';
	export let cardDescription: string = 'Description';
</script>

<section>
	<h2>{cardTitle}</h2>
	<p>{cardDescription}</p>
	<slot />
</section>

<style>
	h2,
	p {
		margin: 0;
	}

	section {
		position: absolute;
		display: flex;
		flex-direction: column;
		justify-content: center;
		gap: 0.5rem;
		height: 100%;
		margin-left: 1rem;
		z-index: 11;
	}
</style>
