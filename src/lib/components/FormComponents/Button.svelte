<script lang='ts'>
	export let btnText: string;
</script>

<button>{btnText}</button>

<style>
	button {
		padding: 1rem;
		background-color: #000000;
		color: #ffffff;
		width: 81%;
		border: none;
        margin: 1rem 0;
        font-weight: bold;
	}
	button:hover {
		background-color: #ffffff;
		color: #000000;
		cursor: pointer;
	}
</style>