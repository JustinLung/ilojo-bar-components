<script type="ts">

    export let storyLink :string;
    export let storyLinkText:string;
    export let height:string;
	export let storyPlateImage :string;
	export let color:string;
</script>

 <div class="container">
    <img src={storyPlateImage } alt="storyPlateImage" style="height: {height};" />
    <div class="centered"><a href="/{storyLink }" style="color: {color};" >{storyLinkText}</a></div>
</div>


<style>

.container {
		position: relative;
		text-align: center;
		color: white;
	
	}
	.centered {
		position: absolute;
		top: 0;
		top: 50%;
		left: 50%;
		transform: translate(-50%, -60%);
	}

    img {
		height: 5rem;	
		
	}

    a {
		text-decoration: none;
		color: var(--light);
		font-size: 1.2rem;
	}

</style>