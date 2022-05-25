<script context="module">
	export const prerender = true;
</script>

<script>
	let srcGuidingJobSeekers = '/guiding-job-seekers/guding-job-seekers.png';
	let srcFindingTalent = '/finding-talent/finding-talent.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
<section class="intro">
	<h1 class="l">
		Hello, I'm Rebecca Norén. Product Designer in Stockholm. Currently working with messaging at <a
			rel="external"
			href="https://www.sinch.com/"
			>Sinch.
		</a>
	</h1>
</section>

<section class="works">
	<h2 class="normal xs">Selected work</h2>
	<div class="works-grid">
		<a sveltekit:prefetch href="/guiding-job-seekers">
			<figure class="item">
				<img
					src={srcGuidingJobSeekers}
					class="rounded"
					alt="Guiding content showing text and a video."
				/>
				<figcaption>
					<p class="uppercase xxs">TRR (2020)</p>
					<h3 class="m">Guiding job-seekers</h3>
				</figcaption>
			</figure>
		</a>
		<a sveltekit:prefetch href="/finding-talent">
			<figure class="item">
				<img
					src={srcFindingTalent}
					class="rounded"
					alt="Search tool for finding candidates to recruit"
				/>
				<figcaption>
					<p class="uppercase xxs">TRR (2019)</p>
					<h3 class="m">Helping employers finding talent</h3>
				</figcaption>
			</figure>
		</a>
	</div>
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: left;
		flex: 1;
	}

	.works {
		margin-top: 100px;
	}

	.works a {
		color: var(--text-color);
	}

	.works-grid {
		display: flex;
		flex-direction: row;
		flex-wrap: wrap;
		justify-content: center;
		flex: auto;
		gap: 20px;
		max-width: 100%;
	}

	.works h2 {
		margin-bottom: 40px;
	}

	.works-grid .item {
		padding: 0px;
		margin: 0px;
		max-width: 570px;
		width: auto;
		flex-shrink: 1;
		aspect-ratio: 1 / 1;
		transition: transform 0.2s;
	}

	img {
		object-fit: cover;
		width: 100%;
		height: 100%;
	}

	.intro {
		margin-top: 100px;
	}

	.intro h1 {
		max-width: 750px;
	}

	.intro a {
		color: var(--text-color);
	}

	figcaption {
		text-align: left;
	}

	figcaption h3 {
		margin-top: 10px;
	}

	/* Animations */
	.works-grid .item:hover {
		transform: scale(0.95);
	}

	/* Media Queries */

	@media (max-width: 1025px) {
		.works-grid {
			/* flex-direction: column; */
			align-items: center;
		}

		.works-grid .item {
			max-width: 550px;
			width: 100%;
		}
	}

	@media (max-width: 1225px) {
		.works h2 {
			text-align: center;
		}

		.works-grid {
			/* flex-direction: column; */
			align-items: stretch;
			gap: 64px;
		}

		.works-grid .item {
			max-width: 400px;
		}
	}
</style>
