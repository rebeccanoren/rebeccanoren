<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
	import '../works.css';
</script>

<Header />

<main>
	<slot />
</main>

<footer>
	<a href="https://dribbble.com/rebeccanoren">Dribbble</a>
	<a href="https://linkedin.com/in/rebecca-norén">LinkedIn</a>
	<a href="https://github.com/rebeccanoren">Github</a>
</footer>

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1200px;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer {
		margin-top: 200px;
		display: flex;
		flex-direction: row;
		justify-content: center;
		align-items: center;
		gap: 16px;
		padding: 40px;

		background-color: var(--pure-white);
	}

	footer a {
		font-weight: bold;
		color: var(--accent-color);
	}

	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
</style>
