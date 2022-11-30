<script lang="ts">
	import Image from './Image.svelte';
</script>

<section>
	<form>
		<slot />
	</form>
	<Image imgSource="/assets/images/book-stand.png" />
</section>

<style>
	form {
		width: 25rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 0.2rem;
		background-color: #8c0500;
		margin-right: 2rem;
		border-radius: 20px;
	}
	section {
		display: inline-flex;
		flex-direction: row;
		align-items: center;
		background-color: #8c0500;
		border-radius: 20px;
	}
	@media (max-width: 40rem) {
		form {
			/* width: 15rem; */
			gap: 0.2em;
			margin-right: 0rem;
		}
	}
</style>
