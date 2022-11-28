<script lang="ts">
	export let link: string;
	export let linkTitle: string;
</script>

<a data-sveltekit-reload href={link} class="nav-link">{linkTitle}</a>

<style>
	.nav-link {
		font-size: 1.5rem;
		color: #fff;
		line-height: 1.5;
		text-decoration: none;
		width: fit-content;
	}

	.nav-link::after {
    content: '';
    display: block;
    width: 100%;
    transform: scaleX(0);
    height: 3px;
    left: 0;
    background-color: #fff;
    transform-origin: bottom left;
    transition: transform .5s;
  }

  .nav-link:hover::after {
    transform: scaleX(1);
  }
</style>