<script type="ts">

    export let link:string;
    export let linktext:string;
    export let height:string;
	export let source:string;
	export let color:string;
</script>

 <div class="container">
    <img src={source} alt="goldplate2" style="height: {height};" />
    <div class="centered"><a href="/{link}" style="color: {color};" >{linktext}</a></div>
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