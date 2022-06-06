<script>
	import { page } from '$app/stores';
</script>

<div class="floating-actions">
	<ul>
		<li class:active={$page.url.pathname === '/'}><a sveltekit:prefetch href="/">Home</a></li>
		<li class:active={$page.url.pathname === '/about'}>
			<a sveltekit:prefetch href="/about">About</a>
		</li>
		<li class:active={$page.url.pathname === '/about'}>
			<a href="#top">👆</a>
		</li>
	</ul>
</div>

<style>
	.floating-actions {
		position: fixed;
		z-index: 14;
		background-color: var(--dark);
		bottom: 32px;
		border-radius: 40px;
		box-shadow: 0 1px 18px 0 rgb(0 0 0 / 12%), 0 6px 10px 0 rgb(0 0 0 / 14%),
			0 3px 5px -1px rgb(0 0 0 / 20%);
		left: 50%;
		transform: translateX(-50%);
	}

	ul {
		display: flex;
		list-style-type: none;
		padding: 0 24px;
	}

	li {
		text-decoration: none;
		padding: 5px;
	}

	a {
		color: var(--pure-white);
		text-decoration: none;
		padding: 16px;
		border-radius: 40px;
		font-size: 16px;
	}

	a:hover {
		background-color: var(--pure-white);
		color: var(--dark);
		text-decoration: none;
	}
</style>
