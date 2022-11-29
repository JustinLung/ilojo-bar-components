<script lang='ts'>
	export let placeholder:string;
</script>

<textarea name="content" id="content" cols="30" rows="10" {placeholder} required />

<style>
	textarea {
		min-width: 80%;
		max-width: 80%;
		min-height: 200px;
		max-height: 300px;
        border: none;
	}
</style>