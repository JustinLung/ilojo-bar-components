<script lang="ts">
	export let inputName: string;
	export let placeholder: string;
</script>

<input type="text" id={inputName} {placeholder} required />

<style>
	input {
		width: 80%;
		height: 1.5rem;
		border: none;
		font-size: 0.8rem;
	}
</style>
