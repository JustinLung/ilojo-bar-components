<svg
	class="windowRight"
	width="104"
	height="224"
	viewBox="0 0 101 222"
	fill="none"
	xmlns="http://www.w3.org/2000/svg"
>
	<mask id="path-1-inside-1_38_83" fill="white">
		<path d="M0 0H101V222H0V0Z" />
	</mask>
	<path d="M0 0H101V222H0V0Z" fill="#D7C2A7" />
	<path d="M6 222V0H-6V222H6Z" fill="#A17E53" mask="url(#path-1-inside-1_38_83)" />
	<rect x="23" y="153" width="56" height="41" rx="5" fill="#6C5334" />
	<rect x="23" y="91" width="56" height="41" rx="5" fill="#6C5334" />
	<rect x="23" y="29" width="56" height="41" rx="5" fill="#6C5334" />
</svg>

<style>
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
		.windowRight {
			width: 90px;
			margin-right: 9px;
			margin-bottom: 10px;
		}
	}
</style>
