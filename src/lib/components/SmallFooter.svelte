<script lang="ts">
	export let companyName: string;
</script>

<footer>
	&#169; {new Date().getFullYear()}
	{companyName} &#183; All Rights Reserved
</footer>

<style>
	footer {
		max-width: 80rem;
		margin: 2rem auto 2rem;
	}

	@media (max-width: 80rem) {
		footer {
			text-align: center;
			padding-bottom: 1.5rem;
		}
	}
</style>
