<svg
	class="windowLeft"
	width="104"
	height="224"
	viewBox="0 0 102 222"
	fill="none"
	xmlns="http://www.w3.org/2000/svg"
>
	<mask id="path-1-inside-1_38_78" fill="white">
		<path d="M0 0H102V222H0V0Z" />
	</mask>
	<path d="M0 0H102V222H0V0Z" fill="#D7C2A7" />
	<path d="M96 0V222H108V0H96Z" fill="#A17E53" mask="url(#path-1-inside-1_38_78)" />
	<rect x="23" y="91" width="56" height="41" rx="5" fill="#6C5334" />
	<rect x="23" y="153" width="56" height="41" rx="5" fill="#6C5334" />
	<rect x="24" y="29" width="56" height="41" rx="5" fill="#6C5334" />
</svg>

<style>
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

	@media (max-width: 40em) {
		.windowLeft {
			margin-left: 9px;
			margin-bottom: 10px;
			width: 90px;
		}
	}
</style>
