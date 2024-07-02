<script>
	import Header from '$lib/header/Header.svelte';
	import '../app.css';
	import '../works.css';
	import '../typography.css';
</script>

<div class="app">
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
</div>

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1440px;
		margin: 0 auto;
		box-sizing: border-box;
		margin-bottom: 100px;
	}

	footer {
		padding: 60px;
		display: flex;
		flex-direction: row;
		flex-wrap: nowrap;
		justify-content: space-between;
		background-color: var(--light-blue);
		box-shadow: 0 15px 30px 0 rgb(0 42 102 / 4%), inset 1px 1px 1px 0 hsl(0deg 0% 100% / 90%);
	}

	footer a {
		font-weight: bold;
		color: var(--accent-color);
		padding: 20px;
	}

	footer span {
		padding: 0;
		background-color: transparent;
		font-size: 16px;
	}

	.contact {
		display: flex;
		gap: 8px;
	}

	.contact a {
		margin: 0;
		padding: 0;
	}

	@media (max-width: 1000px) {
		footer {
			padding: 130px 16px;
			flex-direction: column;
			gap: 50px;
			align-items: center;
		}

		.contact {
			flex-direction: column;
			align-items: center;
		}
	}
</style>