<script>
	import FloatingActions from '$lib/floating-actions.svelte';
	let srcPointer = '/pointer.svg';
</script>

<header>
	<nav>
		<a class="vibrate" sveltekit:prefetch href="/">
			<img src={srcPointer} class="shadow" alt="Pointer" /><span>Rebecca Norén</span>
		</a>
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
		max-width: 1440px;
		margin: 0 auto;
	}

	nav a {
		display: flex;
		height: 100%;
		align-items: center;
		padding: 0 1em;
		color: var(--text-color);
		font-size: 0.6rem;
		letter-spacing: 0.02em;
		text-decoration: none;
		scroll-margin-top: 20px;
	}

	nav span {
		background-color: var(--light-purple);
		color: white;
		padding: 6px;
		border-radius: 4px;
		margin-top: 20px;
	}

	nav > :first-child {
		font-size: 1.2rem;
		font-family: 'GT-America';
	}

	nav img {
		max-width: 30px;
		margin-right: 16px;
	}
	.shadow {
		-webkit-filter: drop-shadow(3px 3px 2px rgba(0, 0, 0, 0.7));
		filter: drop-shadow(3px 3px 2px rgba(0, 0, 0, 0.7));
		/* Similar syntax to box-shadow */
	}
	a:hover {
		color: var(--text-color);
	}

	.vibrate {
		-webkit-animation: vibrate 5s ease-out infinite;
		animation: vibrate 5s ease-out infinite;
	}

	@-webkit-keyframes vibrate {
		0% {
			-webkit-transform: translate(0);
			transform: translate(0);
		}
		20% {
			-webkit-transform: translate(4px, -4px);
			transform: translate(4px, 4px);
		}
		40% {
			-webkit-transform: translate(0px, 0px);
			transform: translate(7px, 7x);
		}
		60% {
			-webkit-transform: translate(8x, 8px);
			transform: translate(8x, 8px);
		}
		80% {
			-webkit-transform: translate(-2px, -2px);
			transform: translate(10px, 10px);
		}
		100% {
			-webkit-transform: translate(0);
			transform: translate(0);
		}
	}
	@keyframes vibrate {
		0% {
			-webkit-transform: translate(0);
			transform: translate(2px, 2px);
		}

		10% {
			-webkit-transform: translate(10px, -10px);
			transform: translate(-10px, 3px);
		}
		20% {
			-webkit-transform: translate(10px, 110px);
			transform: translate(-7px, 6px);
		}
		40% {
			-webkit-transform: translate(2px, 2px);
			transform: translate(10px, 6px);
		}

		50% {
			-webkit-transform: translate(10px, 10px);
			transform: translate(-5px, 500px);
		}
		60% {
			-webkit-transform: translate(-2px, 2px);
			transform: translate(-10px, 799px);
		}
		70% {
			-webkit-transform: translate(-2px, 2px);
			transform: translate(-7px, 5px);
		}
		80% {
			-webkit-transform: translate(-4px, 2px);
			transform: translate(-10px, 10px);
		}
		80% {
			-webkit-transform: translate(-4px, 2px);
			transform: translate(-3px, 10px);
		}
		100% {
			-webkit-transform: translate(4px, -8px);
			transform: translate(0px, 2px);
		}
	}
</style>
