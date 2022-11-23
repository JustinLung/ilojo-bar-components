<button>
	<slot />
</button>

<style>
	button {
		all: unset;
		cursor: pointer;
		background-color: #8c0500;
		border: 1px solid #8c0500;
		color: #ffff;
		padding: 0.5rem 2rem;
		border-radius: 0.2rem;
		transition: 0.3s ease-in-out;
	}

	button:hover {
		background-color: transparent;
		border: 1px solid #8c0500;
		color: #8c0500;
	}
</style>
