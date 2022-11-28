<script lang="ts">
	import CardBody from './CardBody.svelte';
	import CardHeader from './CardHeader.svelte';
	import Tag from './Tag.svelte';
	import TagContainer from './TagContainer.svelte';
	import Button from './Button.svelte';
</script>

<article class="card">
	<CardHeader cardTitle="Ilojo Bar Story" />
	<CardBody
		cardTitle="Ilojo Bar Story"
		cardDescription="Lorem ipsum dolor sit, amet consectetur adipisicing elit. Totam, mollitia."
	>
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
	@media (max-width: 55rem) {
		.card {
			width: 100%;
		}
	}
</style>
