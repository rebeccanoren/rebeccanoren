<script>
	import { page } from '$app/stores';
	import FloatingActions from '$lib/floating-actions.svelte';
</script>

<header>
	<nav>
		<a sveltekit:prefetch href="/" id="top">Rebecca Norén</a>
		<FloatingActions />
	</nav>
</header>

<style>
	header {
		display: flex;
		padding: 20px 10px;
	}

	nav {
		flex: 1;
		display: flex;
		flex-direction: row;
		justify-content: space-between;
		width: 100%;
		max-width: 1200px;
		margin: 0 auto;
	}

	ul {
		position: relative;
		padding: 0;
		margin: 0;
		height: 3em;
		display: flex;
		justify-content: center;
		align-items: center;
		list-style: none;
		background: var(--background);
		background-size: contain;
	}

	li {
		position: relative;
		height: 100%;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 1em;
		color: var(--text-color);

		font-weight: 800;
		font-size: 0.8rem;
		text-transform: uppercase;
		letter-spacing: 0.1em;
		text-decoration: none;
	}

	nav > :first-child {
		font-size: 1rem;
		font-family: 'Grifter';
	}

	a:hover {
		color: var(--text-color);
	}
</style>
