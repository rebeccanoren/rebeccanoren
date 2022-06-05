<script>
	import Header from '$lib/header/Header.svelte';

	import '../app.css';
	import '../works.css';
	import '../typography.css';
</script>

<Header />

<main>
	<slot />
</main>

<footer>
	<div class="social">
		<a href="https://dribbble.com/rebeccanoren">Dribbble</a>
		<a href="https://linkedin.com/in/rebecca-norén">LinkedIn</a>
		<a href="https://github.com/rebeccanoren">Github</a>
	</div>
	<div class="contact">
		<span>Want to get in touch?</span><a href="mailto: hello@rebeccanoren.com"
			>hello@rebeccanoren.com</a
		>
	</div>
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
		padding: 60px;
		display: flex;
		flex-direction: row;
		flex-wrap: nowrap;
		justify-content: space-between;
		background-color: var(--pure-white);
	}

	footer a {
		font-weight: bold;
		color: var(--accent-color);
		padding: 20px;
	}

	@media (max-width: 1000px) {
		footer {
			padding: 130px 50px;
			flex-direction: column;
			gap: 50px;
			align-items: center;
		}
	}
</style>
