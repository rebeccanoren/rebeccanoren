<script context="module">
	export const prerender = true;
</script>

<script>
	let srcGuidingJobSeekers = '/guiding-job-seekers/guding-job-seekers.png';
	let srcFindingTalent = '/finding-talent/finding-talent.png';
	let hoverClass = 'noUnderline';

	let enter1 = false;
	let enter2 = false;
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>
<section class="intro">
	<h1 class="l">Hello, hi 🙋‍♀️</h1>

	<h1 class="m">I'm Rebecca Norén, a strategic Product Designer in Stockholm.</h1>
	<p>My works are just a scroll away.</p>
</section>

<section class="works">
	<h2 class="normal xs">Selected work</h2>
	<div class="works-grid">
		<a sveltekit:prefetch href="/guiding-job-seekers">
			<figure
				on:mouseenter={() => {
					enter1 = !enter1;
				}}
				on:mouseleave={() => {
					enter1 = false;
				}}
				class="item"
			>
				<img
					src={srcGuidingJobSeekers}
					class="rounded"
					alt="Guiding content showing text and a video."
				/>
				<figcaption>
					<p class="uppercase xxs {enter1 ? 'underline' : ''}">TRR (2020)</p>
					<h3 class="m {enter1 ? 'underline' : ''}">Guiding job-seekers</h3>
					<div class="tags">
						<span>JTBD</span> <span>User Story Mapping</span> <span>User Test</span>
					</div>
				</figcaption>
			</figure>
		</a>
		<a sveltekit:prefetch href="/matching-employers-job-seekers">
			<figure
				on:mouseenter={() => {
					enter2 = !enter2;
				}}
				on:mouseleave={() => {
					enter2 = false;
				}}
				class="item"
			>
				<img
					src={srcFindingTalent}
					class="rounded"
					alt="Searching tool to find candidates to recruit"
				/>
				<figcaption>
					<p class="uppercase xxs {enter2 ? 'underline' : ''}">TRR (2019)</p>
					<h3 class="m {enter2 ? 'underline' : ''}">Matching employers with job-seekers</h3>
					<div class="tags">
						<span>User Research</span> <span>Impact Mapping</span> <span>Design Sprint</span>
					</div>
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

	figure {
		width: 100%;
	}
	figure img {
		background-color: rgba(16, 16, 56, 0.03);
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
		max-width: 100%;
	}

	.intro {
		margin-top: 100px;
	}

	.intro h1 {
		max-width: 750px;
	}

	figcaption {
		text-align: left;
	}

	figcaption h3 {
		margin-top: 10px;
	}

	.tags {
		display: flex;
		flex-wrap: wrap;
		margin: 6px;
		gap: 8px;
	}

	span {
		background-color: #e7f0ff;
		color: var(--accent-color);
		padding: 8px 16px;
		border-radius: 20px;
		font-size: 14px;
		white-space: nowrap;
	}

	a:hover {
		text-decoration: none;
	}

	.underline {
		text-decoration: underline;
	}

	/* Animations */
	.works-grid .item:hover {
		transform: scale(0.95);
		text-decoration: none;
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

		span {
			font-size: 12px;
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
