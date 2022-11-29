<script lang='ts'>
	export let imgSource:string;
</script>

<img src={imgSource} alt="formImg" />

<style>
	img {
		width: 15rem;
		height: 100%;
		padding-right: 2rem;
        align-self: flex-start;
        margin-top: 4rem;
	}
	@media (max-width: 40rem) {
		img {
			display: none;
		}
	}
</style>