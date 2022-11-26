<button>
	<slot />
</button>

<style>
	button {
		cursor: pointer;
		background-color: #8c0500;
		color: #ffffff;
		font-weight: 700;
		font-size: 1rem;
		border: 1px solid #8c0500;
		border-radius: 0.3rem;
		padding: 0.5rem 1.5rem;
		transition: 0.3s ease;
	}

	button:hover {
		color: #8c0500;
		background-color: transparent;
	}
</style>
