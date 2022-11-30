<script lang="ts">
	export let labelName: string;
	export let labelText: string;
</script>

<label for={labelName}>{labelText}</label>

<style>
	label {
		width: 80%;
		color: #ffffff;
		font-size: 1rem;
	}
</style>
