<script lang="ts">
	export let link: string;
	export let linkTitle: string;
</script>

<a data-sveltekit-reload href={link} class="nav-link">{linkTitle}</a>
