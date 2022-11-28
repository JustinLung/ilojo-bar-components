<script lang="ts">
	export let cardTitle: string = 'title';
	export let cardImage: string = 'https://placeimg.com/400/225/arch';
</script>

<figure>
	<img src={cardImage} alt={cardTitle} />
</figure>

<style>
	figure {
		padding: 0;
		margin: 0;
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
	}

	img {
		width: 100%;
		border-radius: 0.5rem;
	}
</style>
