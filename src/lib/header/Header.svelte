<script>
	import { page } from '$app/stores';
</script>

<header>
	<nav>
		<a sveltekit:prefetch href="/">Rebecca Norén</a>
		<ul>
			<!-- <li class:active={$page.url.pathname === '/'}><a sveltekit:prefetch href="/">Home</a></li>
			<li class:active={$page.url.pathname === '/guiding-job-seekers'}>
				<a sveltekit:prefetch href="/guiding-job-seekers">Guiding job-seekers</a>
			</li>
			<li class:active={$page.url.pathname === '/finding-talent'}>
				<a sveltekit:prefetch href="/finding-talent">Finding talent</a>
			</li> -->
			<!-- <li class:active={$page.url.pathname === '/about'}>
				<a sveltekit:prefetch href="/about">About</a>
			</li> -->
			<!-- <li class:active={$page.url.pathname === '/todos'}>
				<a sveltekit:prefetch href="/todos">Todos</a>
			</li> -->
		</ul>
	</nav>

	<div class="corner">
		<!-- TODO put something else here? github link? -->
	</div>
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
