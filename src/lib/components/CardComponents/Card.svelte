<script lang="ts">
	import CardBody from './CardBody.svelte';
	import CardHeader from './CardHeader.svelte';
	import Tag from './Tag.svelte';
	import TagContainer from './TagContainer.svelte';
	import Button from './Button.svelte';
	export let cardTitle: string = 'Title';
	export let cardDescription: string = 'Description';
	export let cardImage: string = 'https://placeimg.com/400/225/arch';
</script>

<article class="card">
	<CardHeader>
		<img src={cardImage} alt={cardTitle} />
	</CardHeader>
	<CardBody>
		<h2>{cardTitle}</h2>
		<p>{cardDescription}</p>
		<TagContainer>
			<Tag>Story</Tag>
			<Tag>Dark</Tag>
		</TagContainer>
		<Button>Read More</Button>
	</CardBody>
</article>

<style>
	.card {
		width: 25rem;
		position: relative;
		display: flex;
		border-radius: 0.5rem;
		color: #ffffff;
	}

	.card:before {
		position: absolute;
		background: #000000;
		content: '';
		z-index: 10;
		opacity: 0.5;
		width: 100%;
		height: 100%;
		border-radius: 0.5rem;
	}

	h2,
	p {
		margin: 0;
		padding: 0;
	}

	img {
		width: 100%;
		border-radius: 0.5rem;
	}

	@media (max-width: 55rem) {
		.card {
			width: 100%;
		}
	}
</style>
