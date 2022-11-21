<script lang="ts">
	export let storyImage: string;
	export let storyTitle: string;
	export let altTag: string;
</script>

<section>
	<div class="image-container">
		<img class="storyimage" src={storyImage} alt={altTag} />
	</div>

	<div class="window">
		<img class="window" src="/assets/images/window.svg" alt="window" />
		<img class="windowLeft" src="/assets/images/windowLeft.svg" alt="window" />
		<img class="windowRight" src="/assets/images/windowRight.svg" alt="window" />
		<div class="test" />
	</div>

	<h2>{storyTitle}</h2>
</section>

<style>
	section {
		display: flex;
		justify-content: center;
		align-items: center;
		flex-direction: column;
	}

	.image-container {
		position: absolute;
		width: 205px;
		height: 228px;
	}

	.storyimage {
		width: 100%;
		height: 240px;
		cursor: pointer;
		object-fit: cover;
	}

	.window {
		position: relative;
		cursor: pointer;
	}

	.window:hover .windowLeft {
		transform: rotateY(-180deg);
	}

	.window:hover .windowRight {
		transform: rotateY(180deg);
	}

	.windowLeft {
		position: absolute;
		left: 0;
		bottom: 0;
		z-index: 20;
		margin-left: 11px;
		margin-bottom: 15px;
		transition: transform 1.5s ease-in-out;
		cursor: pointer;
		transform-style: preserve-3d;
		cursor: pointer;
		transform: perspective(200px);
		transform-origin: left;
	}

	.windowRight {
		position: absolute;
		right: 0;
		bottom: 0;
		z-index: 20;
		margin-right: 12px;
		margin-bottom: 16px;
		transition: transform 1.5s;
		cursor: pointer;
		transform-style: preserve-3d;
		cursor: pointer;
		transform: perspective(200px);
		transform-origin: right;
	}

	@media (max-width: 40em) {
		h2 {
			font-size: 16px;
		}

		.window {
			width: 12rem;
		}

		.image-container {
			position: absolute;
			width: 179px;
			height: 196px;
		}

		.windowRight,
		.windowLeft {
			width: 90px;
		}
		.windowRight {
			margin-right: 9px;
			margin-bottom: 10px;
		}

		.windowLeft {
			margin-left: 9px;
			margin-bottom: 10px;
		}

		.storyimage {
			height: 210px;
		}
	}
</style>
